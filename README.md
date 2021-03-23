## EPF RUDN Risk Map Project
Prevention of sun ultraviolets: risk map

### FINAL VERSION:

• GIS Programming project to find vulnerable areas in the world in the case of sun flares.  

• 15/03/2021

• This project has been developed for the Geospatial Programming class of Winter 2021, an international collaboration between two universities, EPF of Sceaux, France and RUDN of Moscow, Russia.

• EPF : https://www.epf.fr/

• RUDN : http://www.rudn.ru

• Author : Clavière-Schiele Paul and Teng Lucia, EPF engineering student in 4th year, Aeronautics and Space major

• Instructor : Naci Dilekli, RUDN Professor, https://github.com/ndilekli/

### DATA ARE FROM:

• See data in Folder « data »

• The Relationship Between PM2.5 and the Action

Spectrum of Ultraviolet Radiation : https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8984296

•	Gridded population: https://sedac.ciesin.columbia.edu/data/set/gpw-v3-population-density/data-download

•	Create a grid map of suns angle for the entire world using https://pysolar.readthedocs.io/en/latest/

• PM2.5: https://sedac.ciesin.columbia.edu/data/set/sdei-global-annual-gwr-pm2-5-modis-misr-seawifs-aod/data-download

### Rasters

![image](https://user-images.githubusercontent.com/80332606/111798793-b2d4e480-88ca-11eb-8b50-2ac32017f31f.png)

### STEPS:

-	We start by normalizing the raster representing the population density and the raster depicting the pollution from PM2.5. 

![image](https://user-images.githubusercontent.com/80332606/112130716-0dbb5400-8bc9-11eb-9066-345d54bdc98f.png)

![image](https://user-images.githubusercontent.com/80332606/112130724-114edb00-8bc9-11eb-9024-9d35c9061f19.png)

-	Then we create a raster representing the value of the solar angle on earth for a given day

![image](https://user-images.githubusercontent.com/80332606/112130736-157af880-8bc9-11eb-8510-65b5e5b17c05.png)

-	We cross the data of the pollution and of the population density to obtain a normalized raster representing the most vulnerable places at every time. The value from the two previous rasters are multiplied, with this method we are obtaining a wider range of value which is handier to use afterward. 

![image](https://user-images.githubusercontent.com/80332606/112130761-19a71600-8bc9-11eb-8ee6-414d0042e249.png)

-	Then we cross this raster with the one giving the solar angle value at a given date. With this final raster, we can see the most vulnerable places in the world at a given date because the value of the angle of the incoming solar UVs. 

![image](https://user-images.githubusercontent.com/80332606/112130781-1f046080-8bc9-11eb-8967-d9d08f408c2a.png)

![image](https://user-images.githubusercontent.com/80332606/112130793-2166ba80-8bc9-11eb-95b5-81030e08463f.png)

-	On this final result, we can see the places where the solar UVs will cause the highest damages to the population.

### USEFULNESS:

Run the code with several parameters, one can choose the date and hour. The final risk map will be given in output. 

![Untitled Diagram (5)](https://user-images.githubusercontent.com/80332606/111800276-14498300-88cc-11eb-98e6-dadc10c40abc.png)

### HOW TO GET HELP:

Contact the author by electronic mail : lucia.teng@epfedu.fr or paul.claviere-schiele@epfedu.fr

### WHO MAINTAINS AND CONTRIBUTES TO THE PROJECT:

Contributor : Paul Clavière-Schiele and Teng Lucia


The project will not be updated after the Final Version release.
