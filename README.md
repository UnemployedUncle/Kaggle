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
3. Folder hierarchy
```
tree
ㄴdata ~ source data
ㄴenv ~ environment
ㄴeda ~ EDA Notebook
ㄴsrc ~ source code
ㄴoutput ~ prediction results
ㄴdocs ~ reference documentations
.gitignore ~ input/data/
```
4. Environment
```
# Create
conda create -n "env_name"
conda activate (env_name)

# Export
conda env export > env/(file_name).yaml
conda env export --no-builds | prep -v "prefix" > env/(file_name).yaml

# Install
conda env create -n (env_name) -f (file_name).yaml

# Update
conda update -n (env_name) -f (file_name).yaml --prune
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
