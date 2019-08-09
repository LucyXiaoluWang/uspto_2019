# Summary

 - This repository contains codes of the following paper: [LINK AND TITLE TO BE PROVIDED](https://)

In this paper, we looked at the potential discrimination by USPTO (United States Patent and Trademark Office) between foreign and domestic inventors. Inventions of foreign origin are about 10 percentage points less likely to be granted a U.S. patent than domestic inventions, controlling for invention quality. This finding adds to the body evidence that patent offices may be discriminating against foreigners, in apparent violation of international patent law. We show that this ‘bias’ against foreigners can be explained almost in full by differences in the quality of patent agents and in the financial resources of the applicants, as well as by the fact that domestic firms fight harder than foreign firms to get their patents granted.

# Structure of This Repository
This repository has been organized into the following directories:
## 1. PATSTAT: 
This folder contains the notebooks for generating the BigQuery tables from the CSV files for the PATSTAT tables.
## 2. Computing_FamilyID: 
This folder contains the notebooks for computing the custom family ID and creating the twin application's table.
## 3. Data_Preparation: 
This folder contains the notebooks and data files for combining different datasets and merging their information. Each notebook is used for creating a different set of features, which we then have used for creating the final dataset.
## 4. Final_Dataset: 
This folder contains the notebooks and data files for creating the final tables. The main notebook for preparing the tables is `Final_Dataset_Preparation`. The steps for predicting names' ethnicity, country of origin, and gender can be also found in this folder.


# Installation

## Cloning the USPTO_2019 repository
```
cd destination/path
git clone https://github.com/rezaho/uspto_2019.git
````

## Installing dependencies
In case you need to run the BigQuery commands, you need to first set-up the Google Cloud console. Please follow the instruction in [Google Big Query Quick Start](https://cloud.google.com/bigquery/docs/quickstarts/quickstart-client-libraries#client-libraries-install-python).

We recommend you to create a new virtual environment using `Conda` or `pip` package managers.
The following code creates a new environment for Conda users using the `requirements.txt` file provided in this repository:
```
# using Conda
conda create --name <env_name> --file requirements.txt

conda activate <env_name>
````
If you prefer using `pip` , you may use the following code:
```
# using pip
pip install -r requirements.txt

```
