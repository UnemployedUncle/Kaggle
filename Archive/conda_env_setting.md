# Setting py env using Anaconda

1.create new env  
```conda create -n "(new_env_name)```

2.export conda env.  
```conda env export --no-builds | grep -v "prefix" > (file_name).yaml```

3a. install conda env using yaml.  
```conda env create -n (env_name) -f (file_name).yaml```

3b. update conda env using yaml.  
```conda update -n (env_name) -f (file_name).yaml --prune```
