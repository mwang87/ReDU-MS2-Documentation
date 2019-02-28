# Analyze Your Data: Coanalysis at GNPS

## Coanalyze your Data: GNPS Molecular Networking

### Example Use Cases
 * **Annotate unknown chemicals** in your data by linking it to annotated chemicals in public data from the same sample type (*e.g.* human urine)
 * **Enhanced context** of chemicals detected in your own data, *e.g.* (bio)chemical transformations, by comparing chemicals detected in public data from the same sample type (*e.g.* human urine)

### Summary
 [Molecular Networking](https://www.nature.com/articles/nbt.3597?WT.ec_id=NBT-201608&spMailingID=52025126&spUserID=ODkwMTM2NjI1NQS2&spJobID=981583612&spReportId=OTgxNTgzNjEyS0) is performed in GNPS. Users can co-analyze their data with public data by selecting files using a simple file selector. The file selector allows one to select (and filter) files based on the sample information provided with every file, and place multiple types of files into one of 6 different groups (*i.e.* G1-G6). A single button click on "Set up GNPS Networking" loads all the files and launches a GNPS molecular job; an email will be sent when the job has finished. Further documentation on GNPS molecular networking is located [here](https://ccms-ucsd.github.io/GNPSDocumentation/).

### Tutorial
 1. Log into a [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash2.jsp) account.
 2. Navigate to the [ReDU-MS2](http://dorresteinappshub.ucsd.edu:5005/) homepage.
 3. Click on the **"Select Data to Coanalyze at GNPS"** text.

 **IMAGE**

 4. Select the files you wish to include in the coanalysis by clicking the desired group button (*i.e.* G1-G6). If you mis-selected a group you must reload the page.
   * The orange buttons in the center of the screen correspond to Sample Information categories.

   **IMAGE**

   * If filter/s are used, they will appear as red box/boxes in the Attribute Filters Panel (upper-right corner) of the page. To remove already selected filters click on the red boxed filter you wish to remove and the item should disappear from Attribute Filters Panel.

   **IMAGE**

   * When files are selected into a group the corresponding button becomes red and the number of files is updated in the Selection Summary Panel (upper-left corner).

   **IMAGE**

 **Example:** The .gif below illustrates the selection of files using a filter based on "human" in Curated_SampleType, and the addition of urine files to group 1 (*i.e.* G1).

  **GIF**

 5. Click on the **Set up GNPS Networking** button (blue) at the bottom of the page (this will take you to GNPS where you will be able to add in your own data along with your pre-selected files from ReDU).
 6. **Add your data** to one of the remaining groups (*i.e.* G1-G6).
 6. Launch the molecular networking job with default parameters or customize parameters. Further documentation on GNPS molecular networking is located [here](https://ccms-ucsd.github.io/GNPSDocumentation/).

### Notes:
 * You must have an account at [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash2.jsp) and be signed in prior to launching a job.
 * The number of groups is currently limited to 6.
 * The suggested limit for molecular networking is a total of **2500 files**.

## Coanalyze your Data: GNPS Library Search

### Example Use Cases
 * **Annotate chemicals** in your data via spectral library matching concurrently with public data from the same sample type (*e.g.* human urine) for further analysis.

### Summary
 Chemical annotation is performed in [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash2.jsp) by comparing MS2 spectra, specifically product ion spectra, with reference MS2 fragmentation patterns (GNPS integrates of the majority of public reference MS2 spectra library). GNPS annotations via spectral reference matching are considered level 2 (putative annotation based on spectral library similarity) or 3 (putatively characterized compound class based on spectral similarity to known compounds of a chemical class) by the 2007 metabolomics standard initiative [PMID: 24039616](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3772505/). The **library search results** are displayed on GNPS which includes the option of downloading a table with every chemical annotation versus the files it was detected in (cells of the matrix reflect detected, 1, or not detected, 0). Further documentation on GNPS library search is located [here](https://ccms-ucsd.github.io/GNPSDocumentation/).

### Tutorial
 1. Log into a [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash2.jsp) account.
 2. Navigate to the [ReDU-MS2](http://dorresteinappshub.ucsd.edu:5005/) homepage.
 3. Click on the **"Select Data to Coanalyze at GNPS"** text.

 **IMAGE**

 4. Select the files you wish to include in the coanalysis by clicking the **Group 1 (G1)** button (this is the only group used for library search; multiple attribute files can be added to this group at a time). If you mis-selected a group you must reload the page.
   * The orange buttons in the center of the screen correspond to Sample Information categories.

   **IMAGE**

   * If filter/s are used, they will appear as red box/boxes in the Attribute Filters Panel (upper-right corner) of the page. To remove already selected filters click on the red boxed filter you wish to remove and the item should disappear from Attribute Filters Panel.

   **IMAGE**

   * When files are selected into a group the corresponding button becomes red and the number of files is updated in the Selection Summary Panel (upper-left corner).

   **IMAGE**

 **Example:** The .gif below illustrates the selection of files using a filter based on "human" in Curated_SampleType, and the addition of urine files to group 1 (*i.e.* G1).

  **GIF**

 5. Click on the **Set up GNPS Library Search** button (blue) at the bottom of the page (this will take you to GNPS where you will be able to add in your own data along with your pre-selected files from ReDU).
 6. **Add your data** to **Group 1 (G1)**
 6. Launch the library search job with default parameters or customize parameters. Further documentation on GNPS library search is located [here](https://ccms-ucsd.github.io/GNPSDocumentation/).

## Notes:
 * You must have an account at [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash2.jsp) and be signed in prior to launching a job.
 * All files must be added to **Group 1 (G1)**; there is no support for multiple groups for library search.
 * The suggested limit for GNPS library search is a total of **5000 files**.

## Coanalyze your Data: Chemical Enrichment Analysis

### Example Use Cases
 * **Explore which chemicals are unique (or common) in your data compared to public data** in order to test or develop hypotheses. *viz.* I see compound A in my blood sample, but it is never found in blood in the public data.

### Summary
Chemical annotation is performed in [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash2.jsp) by comparing MS2 spectra, specifically product ion spectra, with reference MS2 fragmentation patterns (GNPS integrates of the majority of public reference MS2 spectra library). **All chemical annotations are tabulated by Group** (*i.e. G1-G6*) **with the number of files in which a chemical was detected.** Further documentation on GNPS is located [here](https://ccms-ucsd.github.io/GNPSDocumentation/).

### Tutorial
 1. Log into a [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash2.jsp) account.
 2. Navigate to the [ReDU-MS2](http://dorresteinappshub.ucsd.edu:5005/) homepage.
 3. Click on the **"Select Data to Coanalyze at GNPS"** text.
 4. __*TOOL UNDER DEVELOPMENT*__
