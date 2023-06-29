# [Kaggle](https://www.kaggle.com/)

## History
1. [230716_AIReport](https://www.kaggle.com/competitions/2023-kaggle-ai-report)



## 1. Coding Convention
1. Markdown style
2. Camel case (Under bars)
3. Folder name : Platform > LectureName_Lecturer (+ Tags)



## 2. Starting new competition
1. Start/End it with README.md
2. Manage it with GitHub
3. Folder hierarchy(Pipeline)
```
tree
ㄴdata ~ source data
ㄴenv ~ environment
ㄴeda ~ EDA Notebook
ㄴsrc ~ source code
    ㄴfeature: feature engineering
    ㄴtrn|model: train
    ㄴval|metric: cross validation
    ㄴtst: test
ㄴoutput ~ prediction results
    ㄴfeature: premade features
    ㄴmodel: model checkpoints
    ㄴsub: submission
    ㄴlog
ㄴdocs ~ reference documentations
.gitignore ~ input/data/
.github ~ issue templates, pull request templates, ...
```
4. Environment
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

5. requirements.txt
```
# Create
pip freeze > requirements.txt

# Install all
pip install -r requirements.txt
```


## 3. README.md Framework
```Markdown
# [Title]()

[Description](#Description)  
[Evaluation](#Evaluation)  
[Contents](#Contents)  
[Reference](#Reference)  

## Description
Timeline

## Evaluation
Submission

## Contents
Data, Code, Model, ...

## Reference
[Ref][id]

[id]: http:// "Optional Title"
```


## Reference
1. 캐글가이드
2. LA오빠
[Title](https://www.youtube.com/watch?v%253DahNx5rqCdfQ)
[Title](https://www.youtube.com/watch?v%253DHqhG7T9UL88)
[Title](https://www.youtube.com/watch?v%253DDk1dznYe5kA)