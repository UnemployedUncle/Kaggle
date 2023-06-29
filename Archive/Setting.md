# Setting.md

Tools: vscode, anaconda, git, github id



# 1. .gitingnore
- No data upload on git, only documents and code (cloud check)



# 2. Git

*Profile > Settings > Developer settings > Personal access tokens

- Task
    - Process: Issue (create task) > Branch > Pull Request > Issue close
        - Issue: task to members with kanban board(Check Projects!)

1. Git clone
    - cmd > git clone "URL"
    - fork? copy every version of the file

2. Git branch
    - git branch -c "new branch"
    - git switch "new branch"

    *Check branch for the issue
    - git fetch
    - git checkout 1-initial-code-for-training-dataset

3. Git commit
    - git add .
    - git commit -m "Message"
    - git pull
    - git push origin "new branch"

4. Building Templates (to-do)
https://soft.plusblog.co.kr/66


# 3. File tree

1. Pipeline
    - input: data file
    - src | notebook: code file
        - feature: feature generation
        - model: train (trn)
        - val | metric: cross evaluation
        - tst: test
    - output
        - feature: 좋은 성능 보이지만 오래 걸리는 경우
        - model: 성능이 좋지만 학습 오래 걸리는 경우
        - prediction
        - sub: submission
        - val: validation
        - log?: log messages
    - internal leaderboard: single & ensemble model perf, feature perf

2. Makefile (to-do)
https://github.com/jeongyoonlee/cat-in-the-dat

3. File naming convention


  - Reference: 
https://www.youtube.com/watch?v=ahNx5rqCdfQ
https://www.youtube.com/watch?v=HqhG7T9UL88
https://www.youtube.com/watch?v=Dk1dznYe5kA



# 4. Anaconda Environment

1. Create conda environment

```
conda create -n "env"
```

2. Starting env
```
source activate "env"
```

3. Export env
```
conda env export > "env.yaml"
```

4. Create new env
```
conda env create -f "env.yaml"
```

5. Remove env
```
conda env remove -n env
```



# 5. Create requirements.txt

1. Create requirements.txt
```
pip freeze > requirements.txt
```

2. Install all
```
pip install -r requirements.txt
```
