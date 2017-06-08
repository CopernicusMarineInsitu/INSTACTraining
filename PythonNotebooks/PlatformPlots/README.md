## PythonNotebooks

Contains the materal for the training courses organised in the frame of the In Situ component of the Copernicus Marine Environment Monitoring Service ([CMEMS](http://marine.copernicus.eu/)). Examples of data downloading and processing with [ipython notebooks](http://ipython.org/notebook.html) (or [Jupyter notebook](http://jupyter.org/)) using [netCDF](http://www.unidata.ucar.edu/software/netcdf/) files:

- Index file as cheatsheet examples:
	* [index_file_donwload.ipynb](./PythonNotebooks/indexFileNavigation/index_file_donwload.ipynb): how to download via ftp index files
	* [index_file_navigation_boundingbox.ipynb](./PythonNotebooks/indexFileNavigation/index_file_navigation_boundingbox.ipynb): how to download via ftp index files and use them to find all platforms contained within a given boundingbox.
	* [index_file_navigation_platformCategory.ipynb](./PythonNotebooks/indexFileNavigation/index_file_navigation_platformCategory.ipynb): how to download via ftp index files and use them to find all platforms of a given category (moorings, drifters, profilers&gliders, etc, vessels).   
<img src="images/indexFileNavBB.png" width="300">

- In situ platform locations examples:
	* [IndexFile_Folium_Visalization.ipynb](./PythonNotebooks/IndexFilePlots/IndexFile_Folium_Visalization.ipynb): folium markers.
	* [read_CMEMS_indexfile.ipynb](./PythonNotebooks/IndexFilePlots/read_CMEMS_indexfile.ipynb): latest Mediterranean platforms location.
	* [plot_positions_latest_global.ipynb](./PythonNotebooks/plot_positions_latest_global.ipynb): latest Global platforms location.
<img align="left" src="images/folium.png" width="300">
<img src="images/locationsMED.png" width="300">
<img src="images/global.png" width="500">

- In situ dataset plots examples:
	* [plot_CMEMS_mooring_NorthWestShelf.ipynb](./PythonNotebooks/PlatformPlots/plot_CMEMS_mooring_NorthWestShelf.ipynb): plots of mooring data
	* [plot_CMEMS_mooring.ipynb](./PythonNotebooks/PlatformPlots/plot_CMEMS_mooring.ipynb): plots of mooring data2
	* [plot_CMEMS_mooring.ipynb](./PythonNotebooks/PlatformPlots/Plot_TimeSeries1.ipynb): plots of mooring data3
	* [plot_CMEMS_vessel.ipynb](./PythonNotebooks/PlatformPlots/plot_CMEMS_vessel.ipynb): plots of vessel data
	* [plot_CMEMS_profiler.ipynb](./PythonNotebooks/PlatformPlots/plot_CMEMS_profiler.ipynb): plots of profilers data
	* [plot_CMEMS_drifter.ipynb](./PythonNotebooks/PlatformPlots/plot_CMEMS_drifter.ipynb): plots of drifters data
<img align="left" src="images/drifter.png" width="300">
<img src="images/mooring.png" width="300">
<img src="images/profiler.png" width="300">
<img align="rigth" src="images/vessel.png" width="300">

- In situ dataset processing examples:
	* time series:
		* [Read_TimeSeries_1.ipynb](./PythonNotebooks/PlatformPlots/Read_TimeSeries_1.ipynb): load variables from a local netCDF file.
		* [Read_TimeSeries_2.ipynb](./PythonNotebooks/PlatformPlots/Read_TimeSeries_2.ipynb): load variables from a file available in a [thredds data server](http://www.unidata.ucar.edu/software/thredds/current/tds/)
		* [Read_TimeSeries_3.ipynb](./PythonNotebooks/PlatformPlots/Read_TimeSeries_3.ipynb): use the [cf-module](http://cfpython.bitbucket.org/) to load a variable knowing its [CF standard name](http://cfconventions.org/standard-names.html).
        
    <img align="left" src="images/timeSeries1.png" width="300">
    <img src="images/timeSeries2.png" width="300">

	* trajectories:
		* [Read_drifter_data_1.ipynb](./PythonNotebooks/PlatformPlots/Read_drifter_data_1.ipynb): read a netCDF file containing a surface drifter trajectory.
		* [Read_drifter_data_2.ipynb](./PythonNotebooks/PlatformPlots/Read_drifter_data_2.ipynb): scatter plot using the data from the previous example.
		* [Read_drifter_data_3.ipynb](./PythonNotebooks/PlatformPlots/Read_drifter_data_3.ipynb): creation of a gridded field using the same data.
    <img align="left" src="images/drifter1.png" width="300">
    <img src="images/drifter2.png" width="300">
    <img src="images/drifter3.png" width="300">

	* grided data:
		* Salinity from CORA [dataset](./PythonNotebooks/PlatformPlots/Read_CORA_dataset.ipynb)
<img src="images/cora.png" width="500">      

- In situ WMS - latest directory (work in progress)


## Legacy

This material has been developed by [Charles Troupin](https://github.com/ctroupin), responsible for in situ tac Communication & Training from 2015-2017. 
Minor contributions from [Paz Rotllan](https://github.com/pazrg).

