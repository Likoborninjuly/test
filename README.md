# Splitty
A web app that provides convenience in splitting the bills among friends. 

## Table of Contents
- [Prerequisite](#prerequisite)
- [Setup](#setup)
- [Code Formatter](#code-formatter)
- [Code Linter](#code-linter)
- [Tests](#tests)
- [Static and Static files](#static-and-static-files)
- [Templates](#templates)
- [Branches and Pull Request](#branches-and-pull-request)
- [Contributions](#contributions)



## Prerequisite 
1) Install [git](https://git-scm.com/downloads)
2) **(optional)** Install [vscode](https://code.visualstudio.com/download)
3) Install [python](https://www.python.org/downloads/) (latest version)

## Setup 
1) Make sure prerequisite has been done
2) Clone this repo and open it with vscode/pycharm (vscode is recommended)
3) Navigate to splitty project `cd <path-to-your-project>/splitty`
4) Run `make install`, this will install pipenv (package manager) and install all dependencies/packages
  **for** **windows**: do `make install-w`, same for `lint-w`, `lint-by-file-w`, others stay the same

5) Run `pipenv shell` to activate the python environment (you will need to activate the environment whenever you code)
    *note: you will have to be in <your_path>/splitty (basically in the directory where the Makefile is) to use `make` command*
6) Lastly, you can run `make run`, this simply runs the app

## Code Formatter
- autopep8 is used for formatting, you can simply run this command
> `make format`
- Alternatively, if you're using vscode, it is recommended to integrate the formatter
    - navigate to `Code > Preferences > Settings`
    - click `workspace` > search for `Formatter`
    - select autopep8 for `Editor:Default Formatters` > tick the box for `Editor: Format On Save`
    - Everytime you save, editor will auto save with formatting


## Code Linter
- Pylint is used for linting, you can simply run this command to lint the whole project
>`make lint`


## Tests
- pytest is used as the test runner
- To keep the tests organized, please only add test file in `tests` folder
- Please prefix your test file with `test_xxx.py` 
- To run all tests, simply run 
`make test`
- To run a single test file, you can run
`pytest <path-to-your-file>`

## Static and Static files
- CSS file is kept within static folder
- Static files are kept using staticfiles, to collect again, run
> `python manage.py collectstatic`

## Templates
- To keep the html files organized, please add any html files to `templates` folder


## Branches and Pull Request
- It is **recommended** to add **JIRA ticket number** to your commit, so JIRA will automatically pick up and update the ticket
e.g. your commit message could look like:
>`feat: [KAN-28] add project setup`
- For simplicity, we'll have a `develop` branch and a `master` branch
- As a good practice
  - always branch out from `master`
  - once dev is complete, merge to `develop` branch, and once it is stable, merge to `master`
  - (if required) get code review from someone, another pair of eyes will be useful
    

## Contributions
This is a group project by group b under University Malaya's WOC7014 2023/24 sem 2. 

**Prepared by:**
1) Wong Hong Han (23062599)
2) Khong Jun Ming (23085546)
3) Liu Xiaoke (23066246)
4) Lee Xing Yii (23072493)
5) Han Aiman Rasyid (17113921)
6) Tan Yong Le (S2164472)

