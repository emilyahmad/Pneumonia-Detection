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