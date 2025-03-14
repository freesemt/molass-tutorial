# Preparation
## Installation

We assume here that you are familiar with [Jupyter Notebook](https://en.wikipedia.org/wiki/Project_Jupyter#Jupyter_Notebook) and have already installed Python and 
relevant packages, e.g., numpy, matplotlib, jupyterlab, etc.

```{note}
Do not confuse "Jupyter Notebook" and "Jupyter Book". The former is a file for programming, while the latter is a tool for publishing.
```

To install the Molass Library package, you can use pip as follows.

```
pip install -U molass
pip install -U molass_legacy
```

<font color="orange">WARNING: These command lines will be available in April, 2025.</font>

```{note}
The molass package currently depends on molass_legacy. This dependency is planned to be removed soon. 
```

## Tools for Jupyter Notebooks

As a tool for programming in Jupyter Notebooks, we recommend either of the following without excluding other alternatives.

* [Jupyter Lab](https://jupyter.org/)
* [Jupyter Extension in VS Code](https://code.visualstudio.com/docs/datascience/jupyter-notebooks)

(download_data_for_this_tutorial)=
## Download Data for this Tutorial

To run and follow the tutorial, download data from the following links.

* [tutorial_data.zip](../../data/tutorial_data.zip)
* [simulated_data.zip](../../data/simulated_data.zip)  (in preparation, currently empty)

You can use one or both of these. They are similar, but not the same. The former is from a real experiment on a few standard proteins, while the latter has been generated using simple, but not realistic, models. See [About Example Data Sets](about_example_data_sets) if you are interested in how they are built.

## Local Settings

Those data sets you have downloaded will be referenced in the tutorial. You are supposed to unzip them and set the unzipped folder locations in a python script named "local_settings.py" placed in one of the upper folders relative to the notebook you run. Copy and modify the code block below to fit to your environment, and save to anywhere like '../../local_settings.py'.

```python
LocalSettings = dict(
    TUTORIAL_DATA=r"D:\MolassData\tutorial_data",   # unzipped data folder
    SIMULATED_DATA=r"D:\MolassData\simulated_data", # unzipped data folder, optional
)
```

You can check your local settings in the next section.