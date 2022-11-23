# Complex_Networks_Master
This repository contains the materials for the computational part of the course 'Complex Networks' of the Master in Complex Systems at IFISC (CSIC-UIB) in Mallorca. 

The course requires no prior knowledge about programming, but is thought to be taken right after, or at the same time, of the theoretical part of the course. In order to follow this course you will have to clone this repository locally on your computer, so that you can work on your own machine. After having it cloned (see next section) you will be able to follow the different lectures by opening the different jupyter notebooks in it, named `Lecture_X.ipynb`, where `X` stands for the number of the lecture. The lectures will consist of going through these notebooks and working out the examples and exercises.

## Cloning this repository locally on your computer

In order to work on the course you can clone this repository from its github page directly (if you have a github account) or you can download the repository as a .gif file and uncompressing it anywhere on your computer where you want the folder to be. To do so go to [this address](https://github.com/IFISC/Complex_Networks_Master), click on the `code` green button and choose the option that best siuts you. The benefit of cloning the repository through your own github account is that you will be able to update the files as I add or modify them between lectures.

## Jupyter lab and virtual environments

For this course we will be using [Jupyter lab](https://jupyter.org/), which is a browser-based platform for developing python projects. Besides that we will also create a [virtual environment](https://docs.python.org/3/tutorial/venv.html), which is a collection of modules that are used for our projects and will be very useful if the modules are being updated with new versions, so that in our virtual environment the code will always work, as it will use the same versions of the modules we have used for generating the code.

### Installing Jupyter lab

Let's start step by step. First of all we need to install jupyter lab in our computer.

#### Linux and Mac

First you need to install python and pip in your computer. Then type on a terminal:

```bash 
pip install jupyter-lab
```

Finally you can launch it from the folder that you want to work in by typing on a terminal (in that folder):

```bash
jupyter lab
```

#### Windows

Follow [this tutorial](https://crib.utwente.nl/manual/pages/jupyterlab-install-guide/index.html).

### Creating a virtual environment for this course

Next step is to create a proper working environment for the code in this course. I called the environment `complex_networks`. It is created using the following commands:

#### Linux and Mac

In a terminal, enter the directory where you have this repository and type

```bash
python -m venv complex_networks
```

Then activate it by typing

```bash
source complex_networks/bin/activate
```
That's great. Now we have a activated virtual environment (you should see your virtual environment name before directory name in parenthesis). Now you should install the packages that we will need for the course:

- ipykernel
- networkx
- numpy
- matplotlib
- pandas

This is done by using the following command

```bash
pip install package_name
```

#### Windows

Open the Start menu and search for `cmd`. Press Enter or click on the result to open a command window—or right-click the option to run it as an administrator, when necessary. Then follow exactly the same instructions as for Linux and Mac, but to activate the environment you will have to type (inside the project directory)

```bash
.\virtualENV\Scripts\activate
```

### Letting Jupyter lab know about our virtual environment

For this you have to type (again in a terminal and in the folder of the project)

```bash
python -m ipykernel install --user --name=complex_networks
```

Now, when you enter Jupyter lab (type `jupyter lab` or `jupyter-lab` on the terminal and press enter), you will find that in the top right corner of the editor you can change the kernel you are using for the computation and it will let you choose the environment we just created (`complex_networks`). 

Now you are all set for starting the course!

## General references and further reading for this course

1. Caldarelli, Guido_ Chessa, Alessandro - Data science and complex networks _ real cases studies with Python-Oxford University Press (2016)
2. Dmitry Zinoviev - Complex Network Analysis in Python_ Recognize - Construct - Visualize - Analyze - Interpret-Pragmatic Bookshelf (2018)
3. Edward L. Platt - Network Science with Python and NetworkX Quick Start Guide_ Explore and visualize network data effectively-Packt Publishing (2019)
4. Filippo Menczer, Santo Fortunato, Clayton A. Davis - A First Course in Network Science-Cambridge University Press (2020)
