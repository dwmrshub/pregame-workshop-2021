# matlab templates

Template_matlab.mat, 2 structures, "Processing" and "Fitting". 

## Processing
* Processing.processed_spectra: table 1024 x 9, fill in with the complex FIDs of the spectra obtained in the end of the processing at each b-value
* Processing.difference_to_GT: table 1024 x 9, fill in with the complex FIDs of the difference between the GT spectra and the spectra obtained in the end of the processing, at each b-value
* Processing.difference_to_GT_freq: table 32 x 9, fill in with the difference between the GT frequency applied and your frequency correction at each repetition for each b-value. 
* Processing.difference_to_GT_phase: table 32 x 9, fill in with the difference between the GT phase applied and your phase correction at each repetition for each b-value. 

## Fitting
* Fitting(i).metab: name of each metab / combination of metab (i) we will look at for the analysis
* Fitting(i).decay_to_b0: table 1x9. Fill in with signal decay (normalised by signal at b0) of metab i
* Fitting(i).relative_conc_b0_tCr: relative concentration to tCr of each metabolite at b0
* Fitting(i).difference_to_GT: table 1x9. Fill in with the difference between the GT signal decay (given in GT folder) and your calculated signal decay of metab i
* Fitting(i).GT_fitted: table 1x9. Fill in with your own fit of the GT signal decay.

# .csv templates

## Processing 
* Processing_Fids.csv: fill in with the complex FIDs of the processed spectra at each b value (9 first lines), and the difference between the GT spectra and your processed spectra (9 last lines). You will add 1024 rows.
* Diff_GT_phase_freq.csv: Fill in with the difference between the GT phase/frequency applied and your correction. 9 first lines frequency, 9 last lines, phase. You will add 32 rows. 

## Fitting
* Fitting.csv: for each metab, it follows the same structure than the matlab structure described just above. Multiplication of lines corresponds to the different b values.n 
