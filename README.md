# ContinuousLST
A continuous dataset of Land Surface Temperature (LST) is vital for climatological and environmental studies. LST can be regarded as a combination of seasonal mean temperature (climatology) and daily anomaly, which is attributed mainly to the synoptic-scale atmospheric circulation (weather). To reproduce LST in cloudy pixels using the code files in this reposetory, time series (2002-today) of cloud-free 1km MODIS Aqua LST images are generated and the pixel-based seasonality (climatology) is calculated using temporal Fourier analysis. To add the anomaly, we are using the NCEP Climate Forecast System Version 2 (CFSv2) model, which provides air surface temperature under both cloudy and clear sky conditions. The combination of the two sources of data enables the estimation of LST in cloudy pixels.
The LSTcont dataset can be used for various applications and studies. Furthermore, datasets for other regions can easily be produced by the GEE platform with the provided code. Due to the significant influence of the temperature seasonality on the algorithm, cautions should be taken when running the code on regions with very low seasonality such as the equatorial regions.
For producing the dataset, one should first run MODIS_TFA_Daily_Mean_Export_2_Assets and MODIS_TFA_Daily_Mean_Export_2_Assets codes to produce the TFAs. Only after both files, MODIS TFA and CFSv2 TFA are ready, Continuous_LST_Daily_Export code file can be used to produce LST_cont. Different code files have been prepared for day, night and daily datasets. 

<a href="https://doi.org/10.5281/zenodo.3952604"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.3952604.svg" alt="DOI"></a>

