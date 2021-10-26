### Ground truth files

Units: phase (rad), frequency (Hz)
For the phase and frequency drifts data, you will find 32x51 values. Data were initially simulated at 51 b-values [0:1:50]. To keep only the b-values of interest you must select the columns 1 2 4 7 11 21 31 41 51, corresponding to the b-values 0 1 3 6 10 20 30 40 50, and therefore work with the expected 32x9 values.   

## matlab

* Phase and frequency drifts: ground_truth_freq_phas_conc.mat, tables all_dyn_phase and all_dyn_freq. Shifts applied to the ground truth data.
* Relative concentrations at b=0 (relative to tCr): ground_truth_freq_phas_conc.mat, structure metab_b0. 
* Grounds truth decay for all metabolites at the 9 chosen b values: GT_decay.mat 

## json and csv 

* Phase and frequency drifts: freq_shifts.csv, phase_shifts.csv. Shifts applied to the ground truth data.
* Relative concentrations at b=0 (relative to tCr): metab_bo.txt, in the format of a json file. 
* Grounds truth decay for all metabolites at the 9 chosen b values: decay_metab.txt (json) 
