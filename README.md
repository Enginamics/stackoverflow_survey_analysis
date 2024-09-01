# stackoverflow_survey_analysis

This is a repository for the [Udacity - Data Scientist](https://www.udacity.com/enrollment/nd025) Course 2 project.

![doc/logo.jpg](doc/logo.jpg)

## Table of Contents

1. [Project Motivation](#project-motivation)
2. [Results](#results)
3. [Files and Folders](#files-and-folders)
4. [Installing](#installing)
5. [Getting started](#getting-started)
6. [Licensing, Authors, and Acknowledgements](#licensing-authors-and-acknowledgements)
7. [Troubleshooting](#troubleshooting)

## Project Motivation

The main objective of this analysis is to get used to the data science process according to [CRISP-DM](https://en.wikipedia.org/wiki/Cross-industry_standard_process_for_data_mining) taught during the [Udacity - Data Scientist](https://www.udacity.com/enrollment/nd025) Course and to apply the acquired knowledge to a real-world problem.

To achieve this, the analysis will use the [Stack Overflow surveys from 2020 to 2024](https://survey.stackoverflow.co/) to address the following three questions:

**When comparing the results from 2020 to 2024 ...**  

- **Question 1: ... did the difficulty of the survey increase over the past four years?**
  - *Relevance*: Understanding changes in survey difficulty over time can help to ensure that any observed trends or patterns in the results are not due to changes in survey complexity.

- **Question 2: ... does the length of the survey have and effect on its experienced difficulty?**   
  - *Relevance*: Evaluating if the length of the survey influences the perceived difficulty helps to understand if the responses are affected by survey fatigue, which could impact the reliability of the results and the quality of the data collected.

- **Question 3: ... did the past four years change job compensation?**   
  - *Relevance*: Examining changes in job compensation over the past four years helps to see trends in salary growth, inflation adjustments, and how economic factors or industry shifts may have influenced compensation practices.

## Results

The results of the analysis can be found in this blog post: [add link here]("")

## Files and Folders

This GitHub repository consists of the following main files and folders:


- `stackoverflow_survey_analysis.ipynb`   
    - Main Jupyter Notebook which describes the survey in detail   
- requirements.txt   
    - This file specifies the dependencies used by the project (see chapter [Installing](#installing) for more details)   
- ./data
    - Folder to store the Stack Overflow survey data from 2020 to 2024 (see chapter [Installing](#installing) for more details)     
- ./doc   
    - Folder which holds additional file(s) used by the documentation   

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
Download the Stack Overflow survey data from **2020**, **2021**, **2022**, **2023** and **2024** to the ./data folder with the following commands   
```shell
cd ./data
```
```shell
curl https://survey.stackoverflow.co/datasets/stack-overflow-developer-survey-2020.zip -o stack-overflow-developer-survey-2020.zip && curl https://info.stackoverflowsolutions.com/rs/719-EMH-566/images/stack-overflow-developer-survey-2021.zip -o stack-overflow-developer-survey-2021.zip && curl https://info.stackoverflowsolutions.com/rs/719-EMH-566/images/stack-overflow-developer-survey-2022.zip -o stack-overflow-developer-survey-2022.zip && curl https://cdn.stackoverflow.co/files/jo7n4k8s/production/49915bfd46d0902c3564fd9a06b509d08a20488c.zip/stack-overflow-developer-survey-2023.zip -o stack-overflow-developer-survey-2023.zip && curl https://cdn.sanity.io/files/jo7n4k8s/production/262f04c41d99fea692e0125c342e446782233fe4.zip/stack-overflow-developer-survey-2024.zip -o stack-overflow-developer-survey-2024.zip
```
- if there are problems with the links, the survey results from 2020 to 2024 can be downloaded [here](https://survey.stackoverflow.co/)

Unzip the survey results into the data folder. The final folder/file structure should look like this:
> ./data/stack-overflow-developer-survey-`2020`/survey_results_public.csv   
> ./data/stack-overflow-developer-survey-`2020`/survey_results_schema.csv   

> ./data/stack-overflow-developer-survey-`2021`/survey_results_public.csv   
> ./data/stack-overflow-developer-survey-`2021`/survey_results_schema.csv  

> ./data/stack-overflow-developer-survey-`2022`/survey_results_public.csv   
> ./data/stack-overflow-developer-survey-`2022`/survey_results_schema.csv  

> ./data/stack-overflow-developer-survey-`2023`/survey_results_public.csv   
> ./data/stack-overflow-developer-survey-`2023`/survey_results_schema.csv  

> ./data/stack-overflow-developer-survey-`2024`/survey_results_public.csv   
> ./data/stack-overflow-developer-survey-`2024`/survey_results_schema.csv   

## Getting started

open analysis either [on github](https://github.com/Enginamics/stackoverflow_survey_analysis/blob/main/stackoverflow_survey_analysis.ipynb) or in your jupyter notebook
```shell
cd /path/to/this/repository
```
```shell
jupyter notebook stackoverflow_survey_analysis.ipynb
```

## Licensing, Authors, and Acknowledgements

Big thank's to Stack Overflow for providing the [survey results](https://survey.stackoverflow.co/)

A special thanks to the [Udacity - Data Scientist](https://www.udacity.com/enrollment/nd025) Course, which made this analysis possible.

## Troubleshooting

If jupyter notebook opens a blank page, try STRG+SHIFT+R to refresh page while ignoring cached files.