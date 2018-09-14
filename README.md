# Geocomputing course (1 day)

These will be [Jupyter Notebooks](http://jupyter.org/) running on [Azure Notebooks](https://notebooks.azure.com/).

Click the `launch azurenb` button to start the interactive Azure Notebooks.

[![Azure Notebooks](https://notebooks.azure.com/launch.png)](https://notebooks.azure.com/import/gh/agile-geoscience/geocomp-1day)

If the Notebook asks you which kernel you want to run, select Python 3.

## Running the notebooks

Hopefully you're already using [Anaconda](https://www.continuum.io/downloads). To make an environment for this notebook, and install `obspy`, you can do this:

```
# Make the environment
conda create -n geocomp anaconda Python=3.6

# Start it
source activate geocomp

# Install obspy and bruges
conda config --add channels conda-forge
conda install obspy -y
conda install geopandas -y
conda install folium -y
pip install bruges

# cd to directory with the notebook in it, then
jupyter notebook
```

