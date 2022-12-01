# BIO 322 Project - Gene Prediction

## Authors:

- Simon Lee (simon.lee@epfl.ch) 
- Léa Goffinet (lea.goffinet@epfl.ch)

## Project Description

In an experiment on epigenetics and memory, Giulia Santoni (from the lab of Johannes Gr¨aff at
EPFL) measured the gene expression levels in multiple cells of a mouse brain under three different
conditions that we call KAT5, CBP and eGFP. In this challenge, the goal is to predict – as accurately
as possible – for each cell the experimental condition (KAT5, CBP or eGFP) under which it was
measured, given only the gene expression levels.

## Python Environment and installing dependencies

```environment.yml ``` - file is included in the repository. Takes dependencies from ```requirements.txt```

To build an environment run the following command:

```conda env create -f environment.yml --name [environment_name] ```

## Data 

The training data contains the normalized counts for 32285 genes in 5000 different cells together
with the experimental condition under which each cell was measured. The test data contains only
the normalized counts and your task is to predict the experimental condition. Data is included in this repository

```../data/train.csv.gz```

```../data/test.csv.gz```

However in our analysis we have saved a new filtered version of our train data which filtered out some genes expressed based on a threshold. In our case we decided to filter out genes that were seen across less than 10% of the cells. Filtering took extremely long so in our analysis we recommend you take advantage of our new dataset:

```../data/filtered_train.csv.gz```

## Methods

#### XG Boost

- Description:

#### Neural Network:

- Description:

## How to run 

All the preprocessing, methods and analysis are contained in the ```cell_prediction_analysis.ipynb``` notebook.

