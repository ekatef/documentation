# PyPSA Earth Documentation

![Size](https://img.shields.io/github/repo-size/pypsa-meets-earth/documentation)

### - Getting ready to change the world!

This repository contains the documentation of PyPSA-Earth including:
- hackathon material in folder `hackathon`  (mandatory for beginners): it contains a 6-step introduction starting from the basics to learn PyPSA-Earth
- sample notebooks to investigate the PyPSA-Earth repository in the folder `notebooks`
- storage of documentation images in the folder `doc`

## Installation

1. Make sure to have installed the PyPSA-Earth package and environment available at [this link](https://github.com/pypsa-meets-earth/pypsa-earth.git)

2. Open your terminal at the parent location where PyPSA-Earth has been installed. Type the following in your terminal to download the package from GitHub:

   ```bash
      .../pypsa/earth/parent/folder % git clone https://github.com/pypsa-meets-earth/documentation.git
   ```

## 1. Hackathon material

Expected experience level: Beginner  
Duration hackathon: 3 hours  
Duration extra DIY exercises: 5 hours

Content:
------------
Slides and jupyter notebook examples are provided in the folder `hackathon`. While there is a lot of theory and text, we always recommend to code & check out stuff where possible. Small examples also help you to "do rather than only observe".

- Full GitHub workflow exercise for a PyPSA-Earth contribution
- The architecture of PyPSA-Earth on GitHub
- Development tools, requirements and installation of PyPSA-Earth
- 3 ways of Snakemake executions and introduction to debugging
- Code-Dev story on efficient vs. poor code and the role of discord
- Guideline on "How to add to need regions to PyPSA-Earth"
- Wrap-up - Hackathon-slides.pdf

### List of selected self-learning material
Aim: We provide a couple of links to efficient self-learning material
- [Fundamentals of energy economics and energy systems](https://nworbmot.org/teaching.html), great open lecture materials from Tom Brown
- [Unix-Shell](https://swcarpentry.github.io/shell-novice/), the Unix shell is fundamental to a wide range of advanced computing tasks, including high-performance computing
- [Python Dojo](https://www.youtube.com/playlist?list=PLBZBJbE_rGRWeh5mIBhD-hhDwSEDxogDg), a series of Python videos for absolute beginners
- [PyPSA examples](https://github.com/PyPSA/PyPSA/tree/master/examples), that help understanding what PyPSA does. Click on [Binder at the PyPSA page](https://github.com/PyPSA/PyPSA) opens the examples.
- [Atlite examples](https://github.com/PyPSA/atlite/tree/master/examples), that help understanding what Atlite does. Requires to install Atlite and open Jupyter notebooks
- [Snakemake tutorial](https://snakemake.readthedocs.io/en/stable/tutorial/tutorial.html), learn more about the powers of Snakemake

Useful packages to dive deeper into:
- [pandas](https://pandas.pydata.org/)
- [geopandas](https://geopandas.org/en/stable/)
- [shapely](https://shapely.readthedocs.io/en/stable/manual.html#introduction)
- [numpy](https://nbviewer.org/github/jrjohansson/scientific-python-lectures/blob/master/Lecture-2-Numpy.ipynb)
- [xarray](http://xarray.pydata.org/en/stable/tutorials-and-videos.html)
- [dask](https://github.com/dask/dask-tutorial)

### List of hero's with a successfull Pull Request (GitHub exercise): 
- Lukas Franken from Germany
- Davide Fioriti from Italy
- Matin Mahmood from United Kingdom
- Max Parzen from Germany
- Thomas Lesieur from France
- Jan Ohlenbusch from Germany
- Taco Niet from Canada
- Pierre McWhannel from Canada
- Mariana Rodríguez-Arce from Costa Rica
- Hana Elattar from Egypt

## 2. Usage examples

You may find helpful to have a look on some usage examples available in the notebooks folder. Good points to start are:

    - [Extraction of the power grid data](https://github.com/pypsa-meets-earth/documentation/tree/main/notebooks/usage_examples/network_validation.ipynb)
    The notebook is focused on retrievement of OSM power data and using them to build a network topology. The extracted data are being pre-processed to obtain a cleaned dataset to be fed into the energy model. Validation of the power grid topology is done using the World Bank data both on the country and the continent levels.

    - [Validation of the Nigeria power system model](https://github.com/pypsa-meets-earth/documentation/tree/main/notebooks/usage_examples/validation_nigeria.ipynb)
    This notebook provides a comprehensive example of the model validation for Nigeria. In particular, we look on extraction and clean-up of the power grid data, assessment of the power demand and installed generators capacities along with examination of the power generation mix.

    - [Evaluation of renewable potential](https://github.com/pypsa-meets-earth/documentation/tree/main/notebooks/usage_examples/build_renewable_profiles.ipynb)
    Here we look on implementation and data used for calculations of the renewable potential to be used by the energy model. Spatial visualization techniques are provided for both raster and clustered plots along with plotting time series.

    - [Assessment of the land availability constraints for renewable generation](https://github.com/pypsa-meets-earth/documentation/tree/main/notebooks/usage_examples/landuse-availability.ipynb)
    That is a demonstration an approach to account land-use restrictions by energy modeling. Spatial data on land type and protected areas are used to evaluate a share of the area where renewable generation can be constructed. After that, we look on implementation of the land-use constrains into a real energy model.

    - [Looking into the optimization results](https://github.com/pypsa-meets-earth/documentation/tree/main/notebooks/usage_examples/solve_network_results.ipynb)
    This notebooks introduces some techniques allowing an in-depth look into optimization results for a given country. We examine the general model structure with it's constrains and check the energy balance discrepancy. Generation and demand time-series are being visualized revealing daily and weekly dynamics. We also propose an approach to draw nice maps demonstrating spatial distribution of the generation capacities.

- We recently updated some [hackathon material](https://github.com/pypsa-meets-africa/pypsa-africa-hackathon) for PyPSA-Africa. The hackathon contains jupyter notebooks with exercises which allows to master tools needed to feel confident about the model. After going through the 1 day theoretical and practical material you should have a suitable coding setup and feel confident about contributing.
- The get a general feeling about the PyPSA functionality, we further recommend going through the [PyPSA](https://github.com/PyPSA/PyPSA/tree/master/examples) and [Atlite](https://github.com/PyPSA/atlite/tree/master/examples) examples.

## 3. Notebooks for data exploration

The folder `notebooks` contains useful notebooks to explore the data of PyPSA-Earth.
The notebooks are self-explainatory and the `pypsa-earth` environment is needed to successfully run the examples.