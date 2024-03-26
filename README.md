# Synthetic Time Series Generation  - Energy Data
This repository attempts to generate synthetic time series based on the residential energy consumer data.

# Data
This dataset includes three years of cleaned hourly data from 3021 commercial smart heat meters installed in Danish residential buildings. The data is screened and interpolated to be equidistant, and missing values are imputed using a weighted moving average combined with a scaling algorithm to obey the data's cumulative trend. Furthermore, hourly consumption is calculated, and the original CSV data files are converted to PARQUET files and repartitioned by the municipality, time resolution, year, and month to save space.

The data directory is divided into the following directories:
  1. Energy
  2. Building
  3. Climate

For additional research, one can access the raw energy data here: https://zenodo.org/records/6563114#.YvTk1PhBwuU

# References
[Three years of hourly data from 3021 smart heat meters installed in Danish residential buildings](https://doi.org/10.1038/s41597-022-01502-3)
