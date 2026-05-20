# Quick \& Dirty Pandas Installation Guide (Windows 11)

## 1\. Install Python

Download Python:

[https://www.python.org/downloads/windows/](https://www.python.org/downloads/windows/)

During installation:

* Check: `Add Python to PATH`
* Click: `Install Now`

## 2\. Verify Installation

Open:

* PowerShell
* OR Command Prompt (`CMD`)

Run:

```
python --version
pip --version
```

If both commands show version numbers, Python and pip are installed correctly.


## 3\. Install pandas

Run:

```
pip install pandas
```

## 4\. Optional but Recommended

Install Jupyter Notebook + Excel support:

```
pip install jupyter openpyxl
```

## 5\. Test pandas

Start Python:

```
python
```

Then type:

```python
import pandas as pd

df = pd.DataFrame({"Name": \["Alice", "Bob"]})
print(df)
```

If the table prints successfully, pandas is working.

Exit Python:

```python
exit()
```

## 6\. Universal Setup Command

For most data/automation projects, install everything at once:

```
pip install pandas openpyxl jupyter matplotlib
```

This installs:

* `pandas` → data analysis
* `openpyxl` → Excel support
* `jupyter` → notebooks
* `matplotlib` → charts/plots

## Troubleshooting

### "python is not recognized"

Python was probably not added to PATH.

Fix:

* Reinstall Python
* Make sure `Add Python to PATH` is checked during setup


### Upgrade pip

```
python -m pip install --upgrade pip
```

## Recommended Workflow

cd Desktop

mkdir my\_project

cd my\_project

pip install pandas
