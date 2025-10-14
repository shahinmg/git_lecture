# gentle introduction to git and github

Some commands to easily copy and paste

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
