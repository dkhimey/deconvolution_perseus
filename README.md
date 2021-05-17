# Perseus Deconvolution

## Jupyter Notebook Files:

- ### 0. IC 348 and NGC 1333 Datasets
    Applying various cuts to initial dataset to obtain the NGC 1333 and IC 348 star data.

- ### 1. Rotational Velocity Deconvolution
    Comparing results to rotational velocity findings of IN-SYNC by [Foster et al. 2015](https://ui.adsabs.harvard.edu/abs/2015ApJ...799..136F/abstract) and [Cottaar et al. 2015](https://ui.adsabs.harvard.edu/abs/2015ApJ...807...27C/abstract) using the [extreme deconvolution algorithm](https://www.astroml.org/book_figures/chapter6/fig_XD_example.html).

- ### 2. Full Deconvolution
    Running the deconvolution dataset on the x, y, z coordinates and u, v, w velocities for each cluster. Exported results used in notebook #3.

- ### 3. Cluster Dust Clippings
    Creating 1-sigma ellipses around each cluster using coordinates found in notebook #2. Clipping the Perseus dust data to produce datasets containing dust in only IC 348 and NGC 1333.

- ### 4. Dispersion and Virial Theorem Calculations
    Calculating gas masses from dust clippings and determining if each cluster is bound to the Perseus Cloud.

## Data Files:

- ### kounkel_2019_apogee.csv
    Original dataset containing stars from [Kounkel et al. 2019](https://ui.adsabs.harvard.edu/abs/2019AJ....157..196K/abstract), cross matched with stars from the Gaia EDR3 survey.

- ### perseus_3d_cutout.fits
    Original Perseus dust data from [CITATION]().

- ### ic348_kounkel_mask.fits / ngc1333_kounkel_mask.fits
    Masks produced using the [glue](http://docs.glueviz.org/en/stable/). The full star dataset was overlayed on the perseus dust data and the stars in the group around each cluster were selected. These data sets were used to produce the individual IC 348 and NGC 1333 datasets in notebook #0.

- ### ic348_apogee.csv / ngc1333_apogee.csv
    Datasets produced in notebook #0 using various cuts to the data. These will be used throughout the analysis as the NGC 1333 and IC 348 star data.

- ### deconvolution_results.csv
    Exported results of the extreme deconvolution algorithm performed in notebook #2. Results are used to create 1-sigma ellipses around each cluster in notebook #3.

- ### perseus_ic348_mask_ellipse.fits / perseus_ngc1333_mask_ellipse.fits
    Masks for the Perseus dust data that include the dust around the IC 348 and NGC 1333 clusters. Produced and used in notebook #3.

- ### perseus_ic348_only.fits / perseus_ngc1333_only.fits
    Dust data, obtained from the full Persus dust dataset, containing only the dust surrounding IC 348 and NGC 1333. Produced in notebook #3 and used notebook #4.