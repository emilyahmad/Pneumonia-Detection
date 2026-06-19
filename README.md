# Pneumonia-Detection

Classification project

## Steps

### Setup python environment

Make sure your virtual environment (venv) is the same python version as your kernel
You can deactivate your current python

```
deactivate
```

and specify your venv's python version

```
python3.13.9 -m venv aimi2
source aimi2/bin/activate
```

You can troubleshoot by running the following cell

```
import sys
print(sys.executable)
```

Missing any libraries? (ModuleNotFoundError)

```
pip install
```

(numpy, pandas, matplotlib, pillow)
| Name | Type | Purpose |
| -- | -- | -- |
| os | Library | paths |
| numpy | Library | Arrays, CPU |
| pandas | Library | EDA, csvs |
| matplotlib | Library | graphs, evaluation |
| pillow | Library | idk but used in image processing |

### Upload datasets

Didn't want to mess with LFS, download (datasets here)[https://drive.google.com/drive/u/0/folders/1FSBTHuFT334lwBgJK21KYY7_JE-aSY0f]

### Data exploration
