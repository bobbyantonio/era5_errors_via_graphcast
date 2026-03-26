# era5_errors_via_graphcast
Code for analysis / plotting for the manuscript "Error in ERA5 2m Temperature identified using GraphCast"


# Data

All the data I've been using should be saved in `/network/group/aopp/predict/HMC007_CHRISTENSEN_GRAPHCAS`. The era5_download script can be used to download ERA5 data, eg from https://cds.climate.copernicus.eu/datasets/reanalysis-era5-single-levels?tab=download although you'll probably have to provide credentials.

# Notebooks

All the code used to generate the plots, to calculate the statistics and to justify any of the claims made in the paper should all be in `final_plots.ipynb`. 

I've done a basic job of cleaning up some of the other notebooks used in the project, just in case you need to go back and see how I did something. I haven't tested all the code again in these notebooks, so there's a chance that some data files have moved/been deleted since, but hopefully it's obvious what is needed.

1. `initial_stamp_map_plots` Contains a bunch of stamp map plots of different variables, that we used at the start to see if there was anything interesting happening when the error appeared.

2. `looking_for_corr_with_other_vars` Lots of time series and scatter plots, again looking for correlations with other variables. Also has all the satellite data I've been working with.

3. `observational_data` Details about loading and processing land observation data (METAR and SYNOP). Also contains the work I did trying to work out what days observations over this area would be rejected, as per the document that Massimo sent (https://www.ecmwf.int/en/elibrary/81624-ifs-documentation-cy49r1-part-ii-data-assimilation, Section 9.2)

4. `summary_figures` Contains a couple distribution and time series plots that I used when making my summary overleaf doc

5. `other_areas_and_times` Lots of plots from the end of the project, comparing the data over Ethiopia to other areas etc.
