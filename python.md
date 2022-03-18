# Python

**Autor: **Christian Grubmüller

**Datum:** 18.03.2022

## Alle packages deinstallieren [^1]

```bash
# creates a virtualenv
python3 -m venv venv

# activates the virtualenv
source venv/bin/activate

# verify its working
which python

# freeze dependencies into requirements.txt
pip3 freeze > requirements.txt

# install all dependencies from requirements.txt
pip3 install -r requirements.txt

# delete all installed dependencies from venv / the environment
pip3 freeze | xargs pip uninstall -y

# list all installed dependencies
pip3 list
```



## Quellen

[^1]: "virtualenv Cheatsheet" [online](https://aaronlelevier.github.io/virtualenv-cheatsheet/)
