# [Titanic - Machine Learning from Disaster]([Title](https://www.kaggle.com/competitions/titanic/overview))

## Internal Leaderboard

[Description](#Description)
[Evaluation](#Evaluation)
[Contents](#Contents)
[Reference](#Reference)

## Description
Revisited the competition to practice building ML pipelines.  
Still a great starting point for everyone.

## Evaluation
1. Metric  
![Accuracy](https://wikimedia.org/api/rest_v1/media/math/render/svg/7bfe40cea126a04004b82f729cf7df1ec435fbf6)

2. Submission
    - PassengerId
    - Survived (1 for survived, 0 for deceased)

## Contents
1. data
    - train.csv
    - test.csv
    - gender_submission.csv

2. code




3. env
    1. conda env
    2. requirements.txt

```
# Conda Environment
## Create
conda create -n "env_name"
conda activate (env_name)

## Export
conda env export > env/(file_name).yaml
conda env export --no-builds | prep -v "prefix" > env/(file_name).yaml

## Install
conda env create -n (env_name) -f (file_name).yaml

## Update
conda update -n (env_name) -f (file_name).yaml --prune

## Remove
conda env remove -n (env_name)
```

```
# Create
pip freeze > requirements.txt

# Install all
pip install -r requirements.txt
```


## Reference
[Baseline][baseline]  
[Data Analytics][dataAnalytics]
[Fun Approach][familyPred]

[baseline]: https://www.kaggle.com/code/benhamner/random-forest-benchmark-r
[dataAnalytics]: https://www.kaggle.com/code/startupsci/titanic-data-science-solutions
[familyPred]: https://www.kaggle.com/code/erikbruin/titanic-2nd-degree-families-and-majority-voting