# py-ready

Python project template

## Table of Contents

- [Overview](#Overview)
  - [Purpose](#Purpose)
- [Prototyping](#Prototyping)
- [Environment](#Environment)
  - [Pipenv](#Pipenv)
  - [Setting up a project](#Setting-up-a-project)

## Overview

Python has become one of the most widely used programming languages in the developer community.

### Purpose

The purpose of this template is to help you get started with general-purpose projects developed with Python.

## Prototyping with Jupyter Notebooks

During project development with Python, you will need to spend a few hours prototyping functions. The Jupyter Notebook is an open-source web application that allows you to create and share documents containing live code, equations, visualizations, and narrative text. Also, you can divide your code into logical blocks and execute them independently, as well as being able to save those blocks and return to them later. I'm using it because its features happen to align well with prototyping tasks.

Jupyter is not specific to python, so the recommendation is to install it in such a way that it is available for your entire system, outside of isolated development environments.

To install Jupyter on your system run:

```
python -m pip install --user jupyter
```

## Environment

Pipenv has excellent support for managing direct dependencies while keeping track of a full set of dependency versions that are known to work correctly and ensuring that your environment is kept up to date. That makes it good fit for modern pure Python projects.

### Pipenv

Pipenv is a tool that aims to bring the best of all packaging worlds (bundler, composer, npm, cargo, yarn, etc.) to the Python world.

If you already have Python and pip, you can easily install Pipenv into your home directory:

```
pip install --user pipenv
```

### Setting up a project

The first step is to go to the directory of the project in which you are going to work. Then declare a new isolated development environment with ipykernel.

```
pipenv install ipykernel --dev
pipenv run ipython kernel install --user --name=yourprojectname
```
