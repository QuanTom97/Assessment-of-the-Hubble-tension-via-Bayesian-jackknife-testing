# Resources for Assessing the Hubble Tension via Bayesian Jacknife Testing

This repository contains all resources, data, and code used for the analysis in the accompanying paper.  
It provides ready-to-run scripts and organised folders for testing **early vs late Universe hypotheses** and for **Estimating $H_0$**.  

---

## Early vs Late Universe
This corresponds to figure 5 in the paper. 
Located in the `early_vs_late/` folder.  
This section includes two subfolders:

- `z_gt_2/` – tests restricted to $z > 2$ measurements.  
- `z_gt_0.2/` – tests restricted to $z > 0.2$ measurements.  

Each folder contains the four hypotheses (ready-to-run):

1. **Hypothesis 1:** Early Universe is biased  
2. **Hypothesis 2:** Late Universe is biased  
3. **Hypothesis 3:** Both are biased  
4. **Hypothesis 4:** Neither is biased  

### Summary file
A summary script is provided which automatically plots the **posterior distributions** for each hypothesis in both redshift categories.  
This section also contains code for generating the violin plots and threshold plots (as presented in the paper).  

---

## Physical-model plots (violins + threshold histograms)
This corresponds to figures 6 and 7 in the paper.
This section includes a folder that reproduces the **violin plots** and the **threshold-based histograms** used in the paper. The folder also contains the pickle file with the current posterior data in case you only need to change the plot style.

- **Violin plots:** show the distribution of posteriors across all configurations for each hypothesis.
- **Threshold histograms:** for a chosen scenario/hypothesis and a user-specified threshold (e.g. 0.3), this plots how often each data point appears in combinations where the posterior exceeds that threshold.

---

## Bias specifications and $H_0$ measurements plots
This corresponds to figures 2 and 4 in the paper.
The plots for the bias specifications and $H_0$ measurements are included in a dedicated file. These are already set up and should not need modification. 

---

## $H_0$ Marginalisation (Physical Models)
This corresponds to figure 8 in the paper.
Located in the `H0_marginalisation/` folder.  

- Each physical model has its **own script**, preconfigured and ready to run.  
- Chain files are included for convenience so users can **skip rerunning** PolyChord if they prefer.  
- The summary script combines the results across models and includes routines for computing **credible intervals**.   

---

These scripts are pre-configured and should just need running. The only modifications that will be needed is changing the file paths for the H_0 measurement file and also the location of the chain files in the summary files.

---

## $H_0$ measurements file
The file containing the H_0 measurements used in the analysis is also included.

---

## Dependencies

The following are required to run the code:

- **Python** (>=3.8 recommended)  
- **CHIBORG** (with the updated `jk_hyp.py` and `jk_calc.py` files included in this repository)  
- **PolyChord**  
- **anesthetic**  

Installation instructions for these packages can be found in their respective repositories.  

---

## Contact

For questions, issues, or collaboration, please contact:  

**Thomas Hughes**  
tjhughes97@hotmail.co.uk  
