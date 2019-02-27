# Analyze Public Data: Explore Multivariate Analysis of Public Data
 ### Example Use Cases
 * **Explore public data** by comparing the chemicals annotated in samples, analyzed by principal components analysis (PCA), *viz.* human breast milk appears to be most similar to food given their proximity in the PCA score plot.
 * **Begin to explore high-level questions** that remain unanswered when attempting to compare public mass spectrometry data. For example, does urine always look, chemically, like urine year after year, across instruments, across extraction methods, etc?
 
 ### Summary
 The common denominator of all mass spectrometry data is the chemicals detected. In spite of the numerous confounders (*e.g.* instrument type, user, year, and extraction method), the chemicals that are detected and annotated from samples is the ground truth of any experiment. The **MS2 data, specifically product ion scans, are extracted from the public data and analyzed *de novo* in GNPS**, and in doing so provide the chemical annotations based on library spectral matching for each file. **Principal components analysis (PCA)** was used to analyze the results in an unsupervised manner. The results are plotted using Tableau which provides interactive plotting capabilities to explore the data via a PCA score plot (upper panel), a scatter plot of the number of MS2 spectra per file versus how many of those MS2 spectra were annotated (lower-left panel), and a stacked histogram of the number of chemical annotations (lower-right panel).
 
 ### Tutorial
 1. Navigate to the [ReDU-MS2](http://dorresteinappshub.ucsd.edu:5005/) homepage.
 2. Click on the **"Explore Multivariate Analysis of Public Data"** text under the **"Analyze Public Data"** section.
 
 **IMAGE**
 
 3. Each file is plotted as a point in the PCA score plot (upper panel) and colored based on the sample information. Users can change the PC axes displayed using the drop down.

   **GIF**
   
 4. Users can change how the points are colored in the PCA score plot (and correspond plots) based on sample information using the drop down.
      
   **GIF**
 
 5. Users can filter which samples are plotted in the PCA score plot (and correspond plots) based on sample information using the drop down.
      
   **GIF**
 
 6. Plots can be shared and downloaded using the buttons in the lower-right corner of the page.
 
 ### Notes:
 * The panels are interactive and will update when filters and points are colored based on sample information.
 * Detailed information about each file can be obtained by left-clicking the point (this information can be tabulated by clicking the button to the right of the "Exclude" button)
 * The data are updated periodically and will not display your own data immediately - please use the "Multivariate Comparisons" option under the "Analyze Your Data" if you wish to compare your data to the public data.

