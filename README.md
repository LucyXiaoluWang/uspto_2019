# iipp_patent_descrimination_2019


# Installation

## Clone / Download USPTO_2019
```bash
cd destination/path
git clone https://github.com/rezaho/uspto_2019.git
````

## Install Dependencies
In case you need to run the BigQuery commands, you need to first set-up the Google Cloud console. Please follow the instruction in [Google Big Query Quick Start](https://cloud.google.com/bigquery/docs/quickstarts/quickstart-client-libraries#client-libraries-install-python).

We recommend you to create a new virtual environment using `Conda` or `pip` package managers.
The following code creates a new environment for Conda or pip users using the `requirements.txt` file provided in this repository:
```bash
# Creating a new environment using pip

# Creating a new environment using Conda
conda create --name <env_name> --file requirements.txt
````
