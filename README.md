# CMEMS_INSTAC_NoteBooks

Provides examples of data processing with [ipython notebooks](http://ipython.org/notebook.html) (or [Jupyter notebook](http://jupyter.org/)) using [netCDF](http://www.unidata.ucar.edu/software/netcdf/) files.

* plot_CMEMS_*.ipynb: reads and represents data from various types of platforms (mooring, research vessel, profiler, drifter).
 
* Read_TimeSeries_1.ipynb: load variables from a local netCDF file.
* Read_TimeSeries_2.ipynb: load variables from a file available in a [thredds data server](http://www.unidata.ucar.edu/software/thredds/current/tds/)
* Read_TimeSeries_3.ipynb: use the [cf-module](http://cfpython.bitbucket.org/) to load a variable knowing its [CF standard name](http://cfconventions.org/standard-names.html).

* Read_drifter_data_1.ipynb: read a netCDF file containing a surface drifter trajectory.
* Read_drifter_data_2.ipynb: scatter plot using the data from the previous example.
* Read_drifter_data_3.ipynb: creation of a gridded field using the same data.
