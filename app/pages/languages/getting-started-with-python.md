---
title: "Python"
slug: "getting-started-with-python"
category: "languages"
ordinal: 1610
---

If Python isn't already available on your system follow the instructions at [the Hitchhiker's Guide to Python](http://docs.python-guide.org/en/latest/#getting-started) to install Python on your computer.

Exercism currently supports Python3.4, Python3.3 and Python2.7.


## Packages

The [Python Package Index](https://pypi.python.org/pypi) contains thousands of packages.
Pretty much each of them is installable with `pip install packagename`.
If you don't have __pip__ already, [get it now](https://pip.pypa.io/en/latest/installing.html)!

## Running Tests for an Exercise

Execute tests for an exercise with:

```bash
$ cd exercism/python/bob
$ python bob_test.py
```

##  Running Tests for All Exercises

Before running all the tests ensure you have pytest installed:

```bash
$ pip install pytest
```
After pytest is installed all tests can be executed with:

```bash
$ cd exercism/python/
$ py.test
```

## Visual Studio on Windows

Follow the installation instructions for [Python Tools for Visual Studio](https://pytools.codeplex.com/wikipage?title=PTVS%20Installation)

You can either start by creating your own project for working with the Exercism problems or you can download a Visual Studio solution that is already set up.

### Exercism.io Visual Studio Template

This is a Visual Studio template that comes pre-configured to work on the problems in as many languages as Visual Studio supports.

![Solution Explorer](/img/setup/visualstudio/SolutionExplorer.png)

1. Download the [Exercism.io Visual Studio Template](https://github.com/rprouse/Exercism.VisualStudio) from GitHub by clicking the Download Zip button on the page.
2. Unzip the template into your exercises directory, for example `C:\src\exercises`
2. Install the [Exercism CLI](http://help.exercism.io/installing-the-cli.html)
3. Open a command prompt to your exercise directory 
4. Add your API key to exercism `exercism configure --key=YOUR_API_KEY`
5. Configure your source directory in exercism `exercism configure --dir=C:\src\exercises`
6. [Fetch your first exercise](http://help.exercism.io/fetching-exercises.html) `exercism fetch python`
7. Open the Exercism solution in Visual Studio
8. Expand the Exercism.python project
9. Click on **Show All Files** in Solution Explorer (See below)
10. The exercise you just fetched will appear greyed out. Right click on the folder and **Include In Project**
11. Get coding...

![Add files](/img/setup/visualstudio/AddFiles.png)

To run the tests, you can do so at the command line, or within Visual Studio.

![Test Explorer](/img/setup/visualstudio/TestExplorer.png)

## Code Style and Linting

There's a style guide called [PEP8](http://legacy.python.org/dev/peps/pep-0008/) that many Python projects adhere to.
Read it when you get a chance!

If you just want a quick overview of some problems in your code, use [pylint](http://www.pylint.org/)!
It can be pretty picky though, so take its results with a grain of salt.
If you don't agree with one of its points, that's a good topic for a discussion in the comments for your program!

If you'd rather have a tool take care of your style issues, take a look at [autopep8](https://github.com/hhatto/autopep8)!
Run `autopep8 -d mycode.py` to get a diff of the changes it proposes and `autopep8 -i mycode.py` to format the code inplace!

## Recommended learning resources

* [The Python Tutorial](https://docs.python.org/3/tutorial/)
* [Learn Python The Hard Way](http://learnpythonthehardway.org/book/)
* [Think Python](http://www.greenteapress.com/thinkpython/html/index.html)
* [The Python Library Reference](https://docs.python.org/3/library/index.html)
