# stackoverflow_survey_analysis

This is a repository for the `Udacity - Data Scientist` course 2 project.

![doc/logo.jpg](doc/logo.jpg)

## Table of Contents

1. [Project Motivation](#project-motivation)
2. [Results](#results)
3. [Installing](#installing)
4. [Getting started](#getting-started)
5. [Licensing, Authors, and Acknowledgements](#licensing-authors-and-acknowledgements)
6. [Troubleshooting](#troubleshooting)

## Project Motivation

The motivation of this project is to familiarize with the data science process outlined by the CRISP-DM framework during the Udacity Data Science course and to apply the acquired knowledge to a real-world problem.

## Results

The results of the analysis can be found in this blog post: [add link here]("")

## Installing

### If you just want to have a look at the analysis:
open [stackoverflow_survey_analysis.ipynb](https://github.com/Enginamics/stackoverflow_survey_analysis/blob/main/stackoverflow_survey_analysis.ipynb) directly on github (then you don't have to install anything)

### If you want to rerun or extend the analysis:

Make sure [python 3.12.5](https://www.python.org/downloads/release/python-3125/) (or newer) is installed on your machine

Clone this repository to your machine:
```shell
git clone https://github.com/Enginamics/stackoverflow_survey_analysis.git
```
Then create the virtual python environment in the cloned repository
```shell
cd /path/to/this/repository
```
```shell
python -m venv .venv
```
Then activate the virtual environment
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

- 2020  
- 2024   

to the ./data folder
```shell
cd ./data
```
```shell
curl https://survey.stackoverflow.co/datasets/stack-overflow-developer-survey-2020.zip -o stack-overflow-developer-survey-2020.zip && curl https://cdn.sanity.io/files/jo7n4k8s/production/262f04c41d99fea692e0125c342e446782233fe4.zip/stack-overflow-developer-survey-2024.zip -o stack-overflow-developer-survey-2024.zip
```
- if there are problems with the links, the survey results from 2020 and 2024 can be downloaded [here](https://survey.stackoverflow.co/)

Unzip the survey results into the data folder.   
The final folder structure should look like this:
> ./data/stack-overflow-developer-survey-2020/survey_results_public.csv   
> ./data/stack-overflow-developer-survey-2020/survey_results_schema.csv

> ./data/stack-overflow-developer-survey-2024/survey_results_public.csv   
> ./data/stack-overflow-developer-survey-2024/survey_results_schema.csv

## Getting started

open analysis either [on github](https://github.com/Enginamics/stackoverflow_survey_analysis/blob/main/stackoverflow_survey_analysis.ipynb) or in your jupyter notebook
```shell
cd /path/to/this/repository
```
```shell
jupyter notebook stackoverflow_survey_analysis.ipynb
```

## Licensing, Authors, and Acknowledgements

Big thank's to stackoverflow for providing the [survey results](https://survey.stackoverflow.co/)

A special thanks to the Udacity Data Science Course, which made this analysis possible.

## Troubleshooting

If jupyter notebook opens a blank page, try STRG+SHIFT+R to refresh page while ignoring cached files.