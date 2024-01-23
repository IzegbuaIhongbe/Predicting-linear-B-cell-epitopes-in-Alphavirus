# Developing a solution to predict linear B-cell epitopes in Alphavirus

## Abstract

In this study, the aim is to develop an efficient data mining pipeline to predict linear B-cell epitopes in Alphavirus, a genus of mosquito-borne viruses that includes pathogens of medical concern such as Chikungunya. Linear B-cell epitopes are short protein fragments recognized by the immune system and are crucial for the development of vaccines, diagnostic tests, and therapeutic interventions. Given the resource-intensive nature of experimental epitope discovery, computational methods have been employed to prioritize candidates for laboratory characterization. A dataset created by parsing and consolidating data from online databases IEDB, Genbank, and UniProtKB, and explore the trade-off between using smaller amounts of data from similar viruses and larger volumes of data from potentially different viruses. By systematically evaluating exploratory data analysis, data pre-processing, and model selection, our goal is to develop a robust pipeline to potentially predict new, previously unknown epitopes in viruses from the Alphavirus genus.

## Introduction

The identification of linear B-cell epitopes plays a significant role in the development of vaccines, diagnostic tests, and therapeutic interventions against infectious diseases, allergies, and some cancers. Experimentally discovering these epitopes can be laborious and resource-intensive. Over the past three decades, computational methods have been employed to prioritize candidates for laboratory characterization, making the process considerably more efficient.

Alphavirus, a genus of mosquito-borne viruses, includes pathogens of medical concern, such as Chikungunya, which affects millions of people, primarily in the Global South. The potential migration of these viruses to the north due to climate change poses a growing threat. In this study, datasets are utilized which consolidates data from online databases IEDB, Genbank, and UniProtKB. Our objective is to develop an efficient data mining pipeline to potentially predict new, previously unknown epitopes in Alphavirus.

To achieve this goal, systematic approaches towards the data mining process, focusing on exploratory data analysis, data pre-processing, and model selection will be taken. Different training datasets provided, containing increasingly more data from distant relatives of the Alphavirus genus, allowing us to explore the trade-off between using smaller amounts of data from similar viruses and larger volumes of data from potentially different viruses. The aim of this report is to predict new epitopes and, ultimately, the development of effective interventions against Alphavirus-related diseases.

`The step-by-step process is explained in the project notebook`

# Data

3 datasets are used in this project (all datasets can be accessed here [Dataset](https://drive.google.com/drive/folders/1os-L5Ueqx3UdGDAVy8C9ES6DO6LFZbZA?usp=sharing));
1. `df_training_level_1`
2. `df_training_level_2`
3. `df_holdout`

The Data analysis is carried out on dataset 1 with respect to Exploratory data analysis, Data pre-processing, Feature reduction, Data rebalancing, Modelling and Model assessment. The analysis is repeated for dataset 2 and model performance compared for both datasets. The selected pipeline (pre-processing steps + model) are used to predict the classes for the holdout observations (from dataset 3).

The predictions are uploaded as the `model_predictions.csv` file in the repo.

