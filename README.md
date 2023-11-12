# Machine Learning Approaches to Ethical Analysis of Statistics (ICS5110)

Applied ML Assignment collaboration guidelines.

## Install and Commit

Create *python 3.10* env:
`conda create -n aml python=3.10 & conda activate aml`
Install dependencies:
`yes | pip install -r requirements.txt`

## Commiting

When **commiting**, update the requirements:
`jupyter nbconvert --to script ./notebook.ipynb & pipreqs`

## Datasets

Commit datasets as CSV if <10mb, else use LSF.

All CVSs should go to the folder ['./raw_data'](./raw_data)

## ENV configurations

A default `.env` was provided.
Use your own and add it to `.gitignore`.

API connections, environment variables, and other secrets need to go in your .env.
**Do not commit** your .env!