Need to:
+ see if can add kaggle api to git ignore
+ Grab datasets from old computer
+ What was the dataset we used last summer (check if details are on kaggle)
+ Should learn how to use kaggle API instead of just downloading ZIP

# Pneumonia-Detection

Classification, segmentation project

## Steps

### Setup python environment

### Upload datasets

Didn't want to mess with LFS, download [datasets here](https://drive.google.com/drive/u/0/folders/1FSBTHuFT334lwBgJK21KYY7_JE-aSY0f)

### Data exploration

### Set your path

In Notebooks/EDA.ipynb, configure your to point to your .zip file

```
DATA_DIR = Path("")
```


# Troubleshooting tips
Missing any libraries? (ModuleNotFoundError)
Install them within your venv

```
pip install <library>
```

(numpy, pandas, matplotlib, pillow)
| Name | Type | Purpose |
| -- | -- | -- |
| os | Library | paths |
| numpy | Library | Arrays, CPU |
| pandas | Library | EDA, csvs |
| matplotlib | Library | graphs, evaluation |
| pillow | Library | idk but used in image processing |


# Venv md
Make sure your virtual environment (venv) is the same python version as your kernel
You can deactivate your current python

```
deactivate
```

and specify your venv's python version

```
python3.12 -m venv aimi
source aimi/bin/activate
```

You can troubleshoot by running the following cell

```
import sys
print(sys.executable)
```

to run in jupyter notebook

```
jupyter notebook
```

### Git Issues

If you get a warning like "the repository at /path has too many active changes, only a subset of Git features will be enabled"

Exclude your venv and files from installed libraries and packages by add to your .gitignore

```
aimi/
__pycache__/
*.pyc
.ipynb_checkpoints/
.DS_Store
```
