# Analyze Your Data: Multivariate Comparisons
 
 ### Example Use Cases
 * **Check your data against public data** by comparing the chemicals annotated in your samples, analyzed by principal components analysis (PCA), versus chemicals annotated in similar chemicals *viz.* does my urine data look like urine data collected by others?
 * **Explore if interesting differences exist** in your data compared to the public data at the highest-level. For example, does urine from my cohort of diabetes subjects looks similar to other data from different diseases?
 
 ### Summary
 The common denominator of all mass spectrometry data is the chemicals detected. In spite of the numerious confounders (*e.g.* instrument type, user, year, and extraction method), the chemicals that are detected and annotated from samples is the ground truth of any experiment. The **MS2 data, specifically product ion scans, are extracted from the public data and analyzed *de novo* in GNPS**, and in doing so provide the chemical annotations based on library spectral matching for each file. **Principal components analysis (PCA)** was used to analyze the results in an unsupervised manner. The results are plotted using Tableau which provides interactive plotting capabilities to explore the data via a PCA score plot (upper panel), a scatter plot of the number of MS2 spectra per file versus how many of those MS2 spectra were annotated (lower-left panel), and a stacked histogram of the number of chemical annotations (lower-right panel).
 
 ### Tutorial
 1. Log into a [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash2.jsp) account.
 
 perform library search with default parameters.... take job link from results page put into interface - **still need to BUILD**
 
 ?. Navigate to the [ReDU-MS2](http://dorresteinappshub.ucsd.edu:5005/) homepage.

 
 ### Notes:


