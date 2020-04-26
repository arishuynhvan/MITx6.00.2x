# MITx 6.00.2x
[Introduction to Computational Thinking and Data Science - EdX](https://www.edx.org/course/introduction-to-computational-thinking-and-data-4)

## Objectives

1. To record my study 
2. To organize personal notes
3. To maintain accountability with weekly to-do lists and track progress

## Tools

1. Jupyter Notebook
2. Jekyll or some other static pages for blogging
3. Graphic creating and editing software
4. Python 3.5
5. Virtual Environment in anaconda

## Todos

- [ ] Set up a static blog
- [x] Set up local git repo
- [ ] Research and set up for TTD in Python
- [x] Create virtual environment for practice exercises, homework, problems, midterm and exams

## Setup

### [Virtual Environment](https://uoa-eresearch.github.io/eresearch-cookbook/recipe/2014/11/20/conda/)

```conda update conda```

```conda create -n yourenvname python=x.x anaconda```

```source activate yourenvname``` or ```conda activate yourenvname```

Conda activate is faster since conda 4.4

Activating a conda environment modifies the PATH and shell variables to point to the specific isolated Python set-up you created. The command prompt will change to indicate which conda environemnt you are currently in by prepending (yourenvname).

To install extra Python packages ```conda install -n yourenvname [package]```

To deactivate the environment ```conda remove -n yourenvname -all```

#### Name
MITx6002xPractice

#### Directory

##### Environment
```.../MITx6.00.2x/Practice```

##### Third-party libraries
```path_to_your_anaconda_location/anaconda/envs/yourenvname```

##### Check all environments
```conda info -e```

### Jupyter Notebook

#### [Start Jupyter Notebook from within a conda environment](https://stackoverflow.com/a/39070588)

Activate a conda environment in your terminal using source activate <environment name>. This sets the default environment for Jupyter Notebooks. Otherwise, the [Root] environment is the default.

![jupyter notebooks home screen, conda tab, create new environment](https://i.stack.imgur.com/0Qgkx.png)

After activating the conda environment

```python -m ipykernal install --user --name=MITx6002xPractice```

It will return the directory where ipykernel stores the kernelspec of the new virutal environment. The message may look like below

``Installed kernelspec MITx6002xPractice in C:\Users\<username>\AppData\Roaming\jupyter\kernels\mitx6002xpractice``

Then start the jupyter kernal with ```jupyter notebook```

You can also create new environments from within Jupyter Notebook (home screen, Conda tab, and then click the plus sign).

And you can create a notebook in any environment you want. Select the "Files" tab on the home screen and click the "New" dropdown menu, and in that menu select a Python environment from the list.

![check the new environment in jupyter](https://i.stack.imgur.com/otShT.png)

[More info](https://medium.com/@nrk25693/how-to-add-your-conda-environment-to-your-jupyter-notebook-in-just-4-steps-abeab8b8d084)