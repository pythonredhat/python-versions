# Managing Versions on Mac

### to install different versions of python
```bash
pyenv install 3.5.0
pyenv install 3.6.0
```

### to show which versions of python are installed
```bash
* system (set by /Users/username/.pyenv/versions)
  3.5.0
  3.6.0
```

### to find the location of the system python
```bash
which python
```

### to find the locations of the python versions installed by pyenv:
```bash
/Users/username/.pyenv/versions
```

---

# Managing versions in pipenv virtual environment

### if creating a new pipenv virtual environment:
```bash
pipenv --python /Users/username/.pyenv/versions/3.6.0/bin/python
```

### if you are trying to change to python version in an already established pipenv environment, first make sure you have the python version installed on your mac:

```bash
pyenv install 3.6.0
```

then change your Pipfile:
```bash
[requires]
python_version = "3.6"
```

then install the new python version in the virtual environment:
```bash
pipenv --python /Users/username/.pyenv/versions/3.6.0/bin/python
```

### verify your python version in your virtual environment:
```bash
python --version
Python 3.6.0
```

---
# resource:
https://www.ianmaddaus.com/post/manage-multiple-versions-python-mac/

