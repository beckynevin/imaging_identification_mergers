# imaging_identification_mergers

This folder is a collection of tools I used to create the imaging and kinematic classification tool that identifies merging galaxies.

LDA_from_simulations.ipynb will be useful to you if you wish to recreate the LD1 classification. This code directly uses the LDA_img_ratio_statmorph_some_simulation.txt text files to create the LD1 objects for each simulation. It also creates an overall LD1 based on the fraction of major mergers to minor mergers in the universe. Note that since this code uses k-fold cross-validation to estimate the coefficients of LD1 it will not produce identical results each for each run, but they will be consistent within the standard errors on the coefficients.

LDA_from_simulations.ipynb also uses forward stepwise selection to decide on which predictors are necessary to construct LD1 for each simulation.

If you wish to rerun the code that produces the 'LDA_img_ratio_statmorph_some_simulation.txt' files and estimates all the imaging predictor values contained within, use Img_LDA_table-statmorph.ipynb.

If you want to create your own table of imaging predictors from a real survey, use the model of Img_LDA_MaNGA.ipynb.

Lastly, to apply the LD1 decisions from the SUNRISE simulated galaxies to a table created from real galaxies, use LDA_applited.ipynb. This will assign a posterior probability to a given galaxy to determine if it is merging or nonmerging.
