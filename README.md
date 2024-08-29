# stackoverflow_survey_analysis

This is a repository for the `Udacity - Data Scientist` course 2 project.

![doc/logo.jpg](doc/logo.jpg)

## Table of Contents

1. [Installing](#installing)
2. [Getting started](#getting-started)
3. [Project Motivation](#project-motivation)
4. [Results](#results)
5. [Licensing, Authors, and Acknowledgements](#licensing-authors-and-acknowledgements)
6. [Troubleshooting](#troubleshooting)

## Installing

python 3.12.5

```shell
cd /path/to/this/repository
```
```shell
python -m venv .venv
```
Then activate virtual environment
- On Windows:
    ```shell
    .venv\Scripts\activate
    ```
- On macOS/Linux:
    ```shell
    source .venv/bin/activate
    ```
Install all needed packages from requirements.txt into virtual environment
```shell
pip install -r requirements.txt
```
Download the stackoverflow survey data from 

- 2024 
- 2020

to the ./data folder
```shell
cd ./data
```
```shell
curl https://survey.stackoverflow.co/datasets/stack-overflow-developer-survey-2020.zip -o stack-overflow-developer-survey-2020.zip && curl https://cdn.sanity.io/files/jo7n4k8s/production/262f04c41d99fea692e0125c342e446782233fe4.zip/stack-overflow-developer-survey-2024.zip -o stack-overflow-developer-survey-2024.zip
```
- if there are problems with the links, the survey results from 2020 and 2024 can be downloaded [here](https://survey.stackoverflow.co/)

Unzip the survey results into the data folder. The final folder structure should look like this:
> ./data/stack-overflow-developer-survey-2020/survey_results_public.csv

> ./data/stack-overflow-developer-survey-2024/survey_results_public.csv

## Getting started

open analysis in jupyter notebook
```shell
cd /path/to/this/repository
```
```shell
jupyter notebook stackoverflow_survey_analysis.ipynb
```

## Project Motivation

<!-- ToDo adding project motivation here -->

## Results

<!-- ToDo adding link to blog post here -->

## Licensing, Authors, and Acknowledgements

Big thank's to stackoverflow for providing the [survey results](https://survey.stackoverflow.co/)

## Troubleshooting

If jupyter notebook opens a blank page, try STRG+SHIFT+R to refresh page while ignoring cached files.