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
