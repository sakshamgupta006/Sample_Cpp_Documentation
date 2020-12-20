Description
===========
Sample Cpp Documentation is a boiler plate code for creating awesome C++ Documentations.
Please Visit [Read The Docs](https://sample-cpp-documentation.readthedocs.io/en/latest/) for detailed
description and Installation procedure. Your new website will look something very similar.


Installation
============
Sample Documentation can be easily built using the procedure described in the following sections.
You can either use python virtual environment (venv) or Conda to build the documentation.

First, clone the Sample_Cpp_Documentation repository using:

```
    git clone https://github.com/sakshamgupta006/Sample_Cpp_Documentation.git
```

Then install doxygen for your OS:

For Ubuntu you can use:

```
    sudo apt-get install doxygen

```

Using Virtual Env
-----------------

**Step:1 : Create a Virtual Environment**
*************************************
Create a python virtual environment using:

```
    python3 -m venv <NAME_OF_UR_ENV>
```

Activate the virtual environment using:

```
    source <NAME_OF_UR_ENV>/bin/activate
```

**Step:2 : Install Required Libraries**
***********************************
Simply use pip with the requirements.txt file to set up the libraries.

```
    pip install -r requirements.txt
```

If there are some errors using the requirements.txt file, u can also install the 
required libraries using the following command:

```
    pip install breathe sphinx_rtd_theme
```

**Step:3 : Building the code**
***************************
Use the following command to build the documentation. This will create a build folder consisting
of all the html files.

```

    make html
```


Using Conda
-----------

**Step:1 : Create a Conda environment**
***********************************
Please install [Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/) before following the next steps.
You can easily create a conda environment using:

```
    conda create -n <NAME_OF_UR_ENV> python=3.7
```

Here, I am using python 3.7, but the documentation is compatible with all python 3 versions.

Example:

```
    conda create -n cppdocs python=3.7
```

**Step:2 : Install Required Libraries**
***********************************
First activate the previously created conda environment:

```
    conda activate <NAME_OF_UR_ENV>
```
Example:

```
    conda activate cppdocs
```

Alternatively, you can also use the following commands to install the 
required libraries:

```    
    pip install breathe sphinx_rtd_theme
    conda install -c conda-forge breathe
```
**Step:3 : Building the code**
**************************
Use the following command to build the documentation. This will create a build folder consisting
of all the html files.


```    
    make html
```
