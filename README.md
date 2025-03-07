# Git Plugin
A simple Git automation tool that scans a directory for `.git` repositories and runs `git pull`, `git push`, and `git push --tags`.

## Features
- Scans the specified directory for Git repositories
- Automatically pulls the latest changes
- Pushes local commits and tags to the remote repository

## Installation and Setup
Clone the repository:  
```sh  
git clone https://github.com/sidnair2000/git-plugin.git  
cd git-plugin

## Set up a virtual environment (optional but recommended):

python -m venv venv  
source venv/bin/activate  # On Windows use `venv\Scripts\activate`  
pip install -r requirements.txt  

