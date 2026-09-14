# gentle introduction to git and github

Some commands to easily copy and paste

Slides are [here](https://docs.google.com/presentation/d/1MkCPWBuzkbIhUDLKpUXLQZRK6JbxOPtadPqBIEi1ABY/edit?usp=sharing)

## Follow along (optional)

If you want to follow along please install git. If you are on windows I advise using miniconda. Follow the installation instructions [here](https://github.com/shahinmg/git_lecture.git) to install conda. 

In a conda environment (not your base env) install git

```
conda install -c conda-forge git
```

If you have not created an environment in the terminal before, please create a new environment 

```
conda create -n git_lecture -c conda-forge python=3.13 git -y
```

Breif explanation of conda create command 


| Flag / argument | Meaning |
|---|---|
| `conda create` | create a new virtual environment in conda |
| `-n git_lecture` | Short for `--name`. Names the environment `git_lecture` |
| `python=3.13` | specify the version of python you want |
| `-c conda-forge` | Short for `--channel`. conda-forge is a channel where you can install software from and is maintained by the open-source community |
| `git` | installs the package git |
| `-y` | Short for `--yes`. Skips the "Proceed ([y]/n)?" prompt |



Then activate the new environment

```
conda activate git_lecture
```


## git config
```
git config --global user.name "Your Name"
```

```
git config --global user.email "you@example.com" 
```

## git init
```
git init
```

## github command line
```
gh auth login
```

```
gh repo create
```

## python function - calculate the volume of a sphere 

```
import math

def sphere_volume(radius):
  
  if radius < 0:
    raise ValueError("Radius cannot be negative.")
    
  volume = (4/3) * math.pi * (radius ** 3)
  
  return volume
```

The same function but with the zero radius condition commented out
```
def sphere_volume_wrong(radius):
  
  # if radius < 0:
  #   raise ValueError("Radius cannot be negative.")
    
  volume = (4/3) * math.pi * (radius ** 3)
  
  return volume
```

## git revert to a previous commit
```
git revert --no-commit <commit-id>..HEAD
```
