# Multivariate Analysis of Chemical Annotations Provide Context

# Re-analysis of Public Data in ReDU

## Summary
The common denominator of all mass spectrometry data is the chemicals detected. In spite of the numerous confounders (*e.g.* instrument type, user, year, and extraction method), the chemicals that are detected and annotated from samples is the ground truth of any experiment. The **MS2 data, specifically product ion scans, are extracted from the public data and analyzed *de novo* in GNPS**, and in doing so provide the chemical annotations based on library spectral matching for each file. **Principal components analysis (PCA)** was used to analyze the results in an unsupervised manner. The results are plotted using Emperor which provides interactive plotting capabilities to explore the data via a PCA score plot. Using Emperor, the user has the ability to change the plot axes, color points by sample information, and filter which data point are plotted based on sample information.

!!! notes
	- data are updated periodically and will not display recently contributed data immediately

!!! info "Example Use Cases"
	- **Explore public data** by comparing the chemicals annotated in samples, analyzed by principal components analysis (PCA), *viz.* human breast milk appears to be most similar to food given their proximity in the PCA score plot.
	- **Begin to explore high-level questions** that remain unanswered when attempting to compare public mass spectrometry data. For example, does urine always look, chemically, like urine year after year, across instruments, across extraction methods, etc?
 
!!! example "Tutorial"
	1. Navigate to the [ReDU-MS2](https://redu.ucsd.edu/) homepage.
	2. Click on the **"Explore Multivariate Analysis of Public Data"** text under the **"Analyze Public Data"** section.
		![Redu_Homepage_Link_Location](images/public_comparemultivariate_redu_homepage.png)
	3. Each file is plotted as a point in the PCA score plot. Users can change the PC axes displayed using the drop down.
		![Axis Change Image](images/axis_change.gif)
	4. Users can change how the points are colored in the PCA score plot based on a sample information category selected using the drop down menu.
		![Color Points](images/color_change.gif)
	5. Users can filter which samples are plotted in the PCA score plot based on a sample information cateogry using the drop down menu.
		![Sample Filtration](images/filter_samples.gif)

# Co-analysis of Public Data in ReDU

## Summary
The common denominator of all mass spectrometry data is the chemicals detected. In spite of the numerious confounders (*e.g.* instrument type, user, year, and extraction method), the chemicals that are detected and annotated from samples is the ground truth of any experiment. The **MS2 data, specifically product ion scans, are extracted from the public data and analyzed *de novo* in GNPS**, and in doing so provide the chemical annotations based on library spectral matching for each file. **Principal components analysis (PCA)** was used to analyze the results in an unsupervised manner. The results are plotted using Emperor visualization which provides interactive plotting capabilities to explore the data via a PCA score plot. Using the task ID from the GNPS job previously run, your data will be projected on to a precalculated PCA of all ReDU data. 

!!! info "Example Use Cases"
	- **Check your data against public data** by comparing the chemicals annotated in your samples, analyzed by principal components analysis (PCA), versus chemicals annotated in similar chemicals *viz.* does my urine data look like urine data collected by others?
	- **Explore if interesting differences exist** in your data compared to the public data at the highest-level. For example, does urine from my cohort of diabetes subjects looks similar to other data from different diseases?

!!! example "Tutorial"
	1. Log into a [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash2.jsp) account and perfrom a library search. Once the job has finished running, make note of the task ID found in the URL.
		![Find Task ID](images/find_task_id.jpg)
	2. Navigate to the [ReDU-MS2](https://redu.ucsd.edu/) homepage and click "Compare Your Data to Public Data via Multivariate Analysis" under the Analyze Your Data Section.
		![Homepage Image Public Multivariate](images/comparemultivariate_redu_homepage.png)
	3. Enter the task ID of the previously run GNPS job into the bar, and click the "Create PCA".
		![Enter Task ID](images/task_id_entry.jpg)
	4. For cababilities of data exploration tool, please view [Global Multivariate Analysis Documentation](https://mwang87.github.io/ReDU-MS2-Documentation/AnalyzeYourData_MultivariateComparisons/)
