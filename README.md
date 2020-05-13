# data-py

Data Science and ML Cheatsheet for Python

## Setup

### Python

- Install `python3.8`

  `sudo apt install python3.8`

- Update `~/.bashrc`

  `alias python=python3.8` and then `source ~/.bashrc`

- Install version3.8 `venv`

  `sudo apt-get install python3.8-venv`

- Install `python-dev` (needed to build Python extensions)

  `sudo apt-get install python3.8-dev`

### Virtual Environment

- Create a clean virtual environment and activate

  `python -m venv ./venv`

  `source venv/bin/activate`

- Upgrade `pip`

  `pip install --upgrade pip`

- Deactivate virtual environment

  `deactivate`

### Project dependency

- Save installed packages in `requirements.txt`

  `pip freeze > requirements.txt`

- Install project dependencies from the file

  `pip install -r requirements.txt`

### Git

- push from the local `feature` to the remote `feature`:

```bash
git stash save 'message'         # stash local changes
git pull origin master --rebase  # rebase feature to the origin master
git stash pop/apply              # merge local changes into the latest code
                                 # pop` to remove from stash, `apply` to keep
git add <file/directory>         # stage
git commit -m 'message'          # commit
git push --force-with-lease      # push to feature and check for changes too
```
