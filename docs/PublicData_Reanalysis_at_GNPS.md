# Analyze Public Data: Re-analyze Public Data at GNPS

4 data analysis options currently supported in ReDU (details below in the corresponding section):
* Molecular Networking at GNPS
* Library Search at GNPS
* Chemical Enrichment Analysis
* Sample Information Analysis <br>

## Molecular Networking at GNPS

### Example Use Cases
 * **Annotate unknown chemicals** Molecular networking links chemicals based on MS/MS spectra similarity. Files across data sets from the same sample type can be selected easily. One can find an annotation of interest and see the chemicals related to it. For example, if one was interested in the metabolism of drug A, and drug A is known to be in blood samples. One could select blood, urine, and fecal samples to see if metabolites of drug A exist in the public data.

### Summary
 [Molecular Networking](https://www.nature.com/articles/nbt.3597?WT.ec_id=NBT-201608&spMailingID=52025126&spUserID=ODkwMTM2NjI1NQS2&spJobID=981583612&spReportId=OTgxNTgzNjEyS0) is performed in [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash.jsp). Users can re-analyze public data by selecting files using the ReDU file selector. The file selector allows one to select (and filter) files based on the sample information provided with every file, and place multiple types of files into one of 6 different groups (*i.e.* G1-G6). A single button click on "Set Up Re-Analysis with GNPS Networking" loads all the files and begins a GNPS molecular job. Further documentation on GNPS molecular networking is located [here](https://ccms-ucsd.github.io/GNPSDocumentation/).

### Tutorial
 1. Log into a [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash.jsp) account.
 2. Navigate to the [ReDU](https://redu.ucsd.edu/) homepage.
 3. Click on the **"Re-analyze Public Data at GNPS"** text.
 4. Select the files you wish to include in the re-analysis by clicking the desired group button (*i.e.* G1-G6).
   * The orange buttons in the center of the screen correspond to Sample Information categories.
   * If filter/s are used, they will appear as red box/boxes in the Attribute Filters Panel (upper-right corner) of the page. To remove already selected filters click on the red boxed filter you wish to remove and the item should disappear from Attribute Filters Panel.
   * When files are selected into a group the corresponding button becomes red and the number of files is updated in the Selection Summary Panel (upper-left corner).
 5. Click on the **Set Up Re-Analysis with GNPS Networking** button (blue) at the bottom of the page.
 6. Launch the molecular networking job with default parameters or customize parameters. Further documentation on GNPS molecular networking is located [here](https://ccms-ucsd.github.io/GNPSDocumentation/).
 
<img src="/images/File_Selector.gif" height="400" width="500">

 ### Notes
 * You must have an account at [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash.jsp) and be signed in prior to launching a job.
 * The number of groups is currently limited to 6.
 * The suggested limit for molecular networking is a total of **3000 files**.


## Library Search at GNPS

### Example Use Cases
* **Annotate chemicals** in the public data via spectral library matching using custom parameters. Used for generating a list of annotations based on custom parameters for the files included. All files must be in G1.

### Summary
A **GNPS library search** has been performed for all files with sample information in GNPS using default parameters ([found here](https://redu.ucsd.edu/compoundslist)). This option allows users to reanalyze the public data via custom library search parameters. The **library search results** are displayed on GNPS which includes the option of downloading a table with every chemical annotation versus the files it was detected in (cells of the matrix reflect detected, 1, or not detected, 0). Further documentation on GNPS library search is located [here](https://ccms-ucsd.github.io/GNPSDocumentation/).

### Tutorial
 1. Log into a [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash.jsp) account.
 2. Navigate to the [ReDU](https://redu.ucsd.edu/) homepage.
 3. Click on the **"Re-analyze Public Data at GNPS"** text.
 4. Select the files you wish to include in the re-analysis by clicking **Group 1 (G1)**
   * The orange buttons in the center of the screen correspond to Sample Information categories.
   * If filter/s are used, they will appear as red box/boxes in the Attribute Filters Panel (upper-right corner) of the page. To remove already selected filters click on the red boxed filter you wish to remove and the item should disappear from Attribute Filters Panel.
   * When files are selected into a group the corresponding button becomes red and the number of files is updated in the Selection Summary Panel (upper-left corner).
 5. Click on the **Set Up Re-Analysis with GNPS Library Search** button (blue) at the bottom of the page.
 6. Launch the library search job with default parameters or customize parameters. Further documentation on GNPS library search is located [here](https://ccms-ucsd.github.io/GNPSDocumentation/).

<img src="/images/File_Selector.gif" height="400" width="500">

### Notes
 * You must have an account at [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash.jsp) and be signed in prior to launching a job.
 * All files must be added to **Group 1 (G1)**; there is no support for multiple groups for library search.
 * The suggested limit for GNPS library search is a total of **5000 files**.

# Chemical Enrichment Analysis

### Example Use Cases
* **Explore which chemicals have been detected in *a subset of* the public data** in order to test or develop hypotheses, and determine the specific files in the public data that are relevant for follow up analysis. *viz.* I'm interested in the chemical differences between human urine and human blood - what are they?

### Summary
**All chemical annotations that originate from the selected public data are tabulated by group (G1-G6).** Chemical annotation is performed in [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash2.jsp) by comparing MS2 spectra, specifically product ion spectra, with reference MS2 fragmentation patterns (GNPS integrates of the majority of public reference MS2 spectra library). Default library search parameters are used.

### Tutorial
 1. Navigate to the [ReDU](https://redu.ucsd.edu/) homepage.
 2. Click on the **"Re-analyze Public Data at GNPS"** text.
 3. Select the files you wish to include in the re-analysis by clicking the desired group button (*i.e.* G1-G6).
   * The orange buttons in the center of the screen correspond to Sample Information categories.
   * If filter/s are used, they will appear as red box/boxes in the Attribute Filters Panel (upper-right corner) of the page. To remove already selected filters click on the red boxed filter you wish to remove and the item should disappear from Attribute Filters Panel.
   * When files are selected into a group the corresponding button becomes red and the number of files is updated in the Selection Summary Panel (upper-left corner).
 4. Click on the **Launch Chemical Enrichment Analysis** button (blue) at the bottom of the page.

<img src="/images/File_Selector.gif" height="400" width="500">

## Sample Information Analysis

### Example Use Cases
* **Explore associations between chemcials found in *a subset of* the public data** and sample information in order to test or develop hypotheses. The information could be used to guide follow up analysis using public data that might be relevant.

### Summary
**All chemical annotations that originate from the selected public data are tabulated with a button to view the sample information enrichment for each chemical annotated.** Chemical annotation is performed in [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash2.jsp) by comparing MS2 spectra, specifically product ion spectra, with reference MS2 fragmentation patterns (GNPS integrates of the majority of public reference MS2 spectra library). Default library search parameters are used. Sample information enrichment uses the sample information provided for each files by the community and users of ReDU-MS2.

### Tutorial
 1. Navigate to the [ReDU](https://redu.ucsd.edu/) homepage.
 2. Click on the **"Re-analyze Public Data at GNPS"** text.
 3. Select the files you wish to include in the re-analysis by clicking the desired group button (*i.e.* G1-G6).
   * The orange buttons in the center of the screen correspond to Sample Information categories.
   * If filter/s are used, they will appear as red box/boxes in the Attribute Filters Panel (upper-right corner) of the page. To remove already selected filters click on the red boxed filter you wish to remove and the item should disappear from Attribute Filters Panel.
   * When files are selected into a group the corresponding button becomes red and the number of files is updated in the Selection Summary Panel (upper-left corner).
 4. Click on the **Launch Sample Information Association** button (blue) at the bottom of the page.
 5. Click on the **"View Enrichment"** button (orange) on the right side of the page for the chemical annotation of interest. *KNOWN BUG: the number of files does not update to reflect user selection*

<img src="/images/File_Selector.gif" height="400" width="500">
