# msw17002-Integrated-Surface-Dataset-Extraction-for-Small-Domains
Considering at most ~100-300 surface stations from the Integrated Surface Dataset (for 1-4 day intervals), the Python script; reads daily metadata, removes suspect observations, prints hourly observations, then compiles all station meta data into one .csv file. The goal of this script is to conduct an evaluation on surface variables.

Concidered variables (at the moment) for extraction:
2-m temperature (C)
Station pressure (pa)
2-m Dew point temperature (C)
10-m wind speed (m/s)
10-m wind direction (degrees)
Visibility (m)
wx-type (decoded)
2-m Wet-bulb temperature (C: calculated from Stull's equation)
Relative humidity (%: calculated from temperature and dew point)
Specific Humidity (kg/kg: calculated from dew point temperature and station pressure)

Time difference for hourly extraction is set to +-30 minutes. This can be adjusted to +-1 (or anything between +-30 to +-1 minute) minute if desired.
