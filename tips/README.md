## CMEMS INSTAC KEY FACTS

The In Situ component of the Copernicus Marine Environment Monitoring Services (CMEMS INSTAC) comprehends 7 product distribution units:
<img align="left" src="https://github.com/CopernicusMarineInsitu/INSTACTraining/blob/master/images/regions.png" width="300">
1. Global through [ftp1.ifremer.fr](wwz.ifremer.fr/)
2. Artic through [ftp.nodc.no](arctic-roos.org/members/IMR)
3. Baltic through [cmems.smhi.se](http://www.smhi.se/en) 
4. Mediterranean through [medinsitu.hcmr.gr](http://www.hcmr.gr/en/)
5. North West Shelves through [myocean.bsh.de](http://nwsportal.bsh.de/)
6. Black Sea through [vftpmo.io-bas.bg](http://www.io-bas.bg/index_en.html)
7. Iberian-Biscay-Ireland through [arcas.puertos.es](http://ibidataportal.puertos.es/quid.php)

All those distribution units package [in situ data products](http://cmems-resources.cls.fr/documents/PUM/CMEMS-INS-PUM-013.pdf) in netCDF format and distributes each of them in 3 different directories (*):
<img align="right" src="https://github.com/CopernicusMarineInsitu/INSTACTraining/blob/master/images/ftp_struture.png" width="400">
<br>
<br>
* history (long series of observations: one netCDF per platform)
* monthly (latest 5 years of observations: one netCDF per year&month&platform)
* latest ( latest 30 days of observations: one netCDF per year&month&day&platform)

(*) REP data products are distributed just in one (history).

The objective is facilitate the final user access either to large datasets (history), shorten ones (monthly) or just fresh ones (latest); being then up to the user which one targeting (i.e history directory for climate change monitoring; monthlly or latest for model validation etc).

Additional organization is setup for monthly and history directories, where netCDFs are in turn grouped by platform category:
<img align="left" src="https://github.com/CopernicusMarineInsitu/INSTACTraining/blob/master/images/platforms.png" width="400">

1. Moorings
2. Drifters
3. Vessels
4. Profilers-Gliders
5. Etc

<br>
<br>
For managing purposes, next to each of these folders can be found an index file that maps their content:

* history_index.txt - history directory
* monthly_index.txt - monthly directory
* latest_index.txt - latest directory

Every line of those index files (history_index.txt, monthly_index.txt,latest_index.txt) points to each one of the netCDFs contained within its asociated directory by specifying:

1. catalog_id
2. file_name
    * common:
        * region bigram
        * data type format: TS (timeserie) or PR (profile)
        * data type: CT, BO, RF, MO, DB, DC, TE and [more](http://cmems-resources.cls.fr/documents/PUM/CMEMS-INS-PUM-013.pdf)
        * platform code
        * NetCDF file name suffix (.nc)

    * directory-dependent:
        * platform category (lates & history)
        * timestamp: YYYYMMDD (latest),YYYYMM (monthly)
        * optional sub-setting code (history)
        * fixed name (latest)    

<span padding-left="20%"><img src="https://github.com/CopernicusMarineInsitu/INSTACTraining/blob/master/images/naming.png" width="500"></span>

3. geospatial_lat_min
4. geospatial_lat_max
5.  geospatial_lon_min
6. geospatial_lon_max
7.  time_coverage_start
8.  time_coverage_end
9.  provider
10. date_update
11. data_mode
12. parameters 

For non-interactive in situ dataset download, looping over the lines of the index files is advisable. 
<div style="margin: 0 auto"><img src="https://github.com/CopernicusMarineInsitu/INSTACTraining/blob/master/images/index_files.png" width="600"></div>
