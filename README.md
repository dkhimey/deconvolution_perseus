# Perseus Deconvolution

## Jupyter Notebook Files:

- ### 0. Producing IC 348 and NGC 1333 Datasets

- ### 1. Rotational Velocity Deconvolution
    Comparing results to rotational velocity findings of IN-SYNC by Foster and Cottaar.

- ### 2. Full Deconvolution

- ### 3. Gas Mass Calculations

- ### 4. Dispersion Calculations

## Data Files:

- ### kounkel_2019_apogee.csv
    Original dataset containing stars from [Kounkel et al. 2019](https://ui.adsabs.harvard.edu/abs/2019AJ....157..196K/abstract), cross matched with stars from the Gaia EDR3 survey.

- ### perseus_3d_cutout.fits
    Perseus dust data from [CITATION].

- ### ic348_kounkel_mask.fits and ngc1333_kounkel_mask.fits
    Masks produced using the [glue](). The full star dataset was overlayed on the perseus dust data and the stars in the group around each cluster were selected.
    These data sets were used to produce the individual IC 348 and NGC 1333 datasets.

- ### ic348_apogee.csv and ngc1333_apogee.csv
    Datasets produced in "0. Producing IC 348 and NGC 1333 Datasets" using various cuts to the data.

- ### perseus_ic348_mask_ellipse.fits and perseus_ngc1333_mask_ellipse.fits
    Masks for the Perseus dust data that include the dust around the IC 348 and NGC 1333 clusters. Produced in "3. Gas Mass Calculations".

- ### perseus_ic348_only.fits and perseus_ngc1333_only.fits
    Dust data, obtained from the full Persus dust dataset, containing only the dust surrounding IC 348 and NGC 1333.