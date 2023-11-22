# Machine Learning Approaches to Ethical Analysis of Statistics (ICS5110)

Applied ML Assignment collaboration guidelines. Notebook is here: [aml_ICS5110.ipynb](./aml_ICS5110.ipynb).

## Install and Commit

Create *python 3.10* env:
`conda create -n aml python=3.10 & conda activate aml`

Install dependencies from **requirements.txt**:
`yes | pip install -r requirements.txt`

## Commiting

Use pipreqs to help commit dependencies:
- `pip install pipreqs`
- `pip install nbconvert`

When **commiting**, update the requirements from your base folder:
`jupyter nbconvert --to script *.ipynb & pipreqs . --force`

**NB**: the above will generate a file **.py*, this is only needed for pipreqs to capture dependecies. Do not commit (all python files go to the .ignore)

## Datasets

Commit datasets as CSV if <10mb, else use LSF.

All CVSs should go to the folder ['./raw_data'](./raw_data)

## ENV configurations

A default `.env` was provided.
Use your own and add it to `.gitignore`.

API connections, environment variables, and other secrets need to go in your .env.
**Do not commit** your .env!