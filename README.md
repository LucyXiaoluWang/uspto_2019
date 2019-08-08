# USPTO 2019

 - This repository contains codes fot the following papers: [LINK AND NAME TO BE PROVIDED](https://)

In this paper, we looked at the possible discrimination for foreign inventors. Inventions of foreign origin are about 10 percentage points less likely to be granted a U.S. patent than domestic inventions, controlling for invention quality. This finding adds to the body evidence that patent offices may be discriminating against foreigners, in apparent violation of international patent law. We show that this ‘bias’ against foreigners can be explained almost in full by differences in the quality of patent agents and in the financial resources of the applicants, as well as by the fact that domestic firms fight harder than foreign firms to get their patents granted.

# Structure of This Repository
This repository has been organized into the following directory:
1. PATSTAT: Contains the code for generating BigQuery tables from the CSV files of the PATSTAT tables.
2. Computing_FamilyID: Contains the code for computing the custom family ID and creating the twin application's table.
3. Data_Preparation: Contains the code for combining different datasets and merging their information
4. Final_Dataset: Contains the code for the final steps of preparing tables and also using different sources of information including NamSor API and NamePrism API.


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
