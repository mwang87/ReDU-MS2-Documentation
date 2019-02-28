# Analyze Public Data: Reanalysis at GNPS

# Reanalyze Public Data: GNPS Molecular Networking
 
 ### Example Use Cases
 * **Annotate unknown chemicals** linking annotated chemicals in public data from the same sample type (*e.g.* human urine) as different methods will capture different chemical information.
 * **Enhanced context** of chemicals detected in public data, *viz.* chemical differences and similarity between sample types (*e.g.* human urine versus human blood).
 
 ### Summary
 [Molecular Networking](https://www.nature.com/articles/nbt.3597?WT.ec_id=NBT-201608&spMailingID=52025126&spUserID=ODkwMTM2NjI1NQS2&spJobID=981583612&spReportId=OTgxNTgzNjEyS0) is performed in GNPS. Users can reanalyze public data by selecting files using a simple file selector. The file selector allows one to select (and filter) files based on the sample information provided with every file, and place multiple types of files into one of 6 different groups (*i.e.* G1-G6). A single button click on "Set up GNPS Networking" loads all the files and launches a GNPS molecular job; an email will be sent when the job has finished. Further documentation on GNPS molecular networking is located [here](https://ccms-ucsd.github.io/GNPSDocumentation/).
 
 ### Tutorial
 1. Log into a [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash2.jsp) account.
 2. Navigate to the [ReDU-MS2](http://dorresteinappshub.ucsd.edu:5005/) homepage.
 3. Click on the **"Select Data to Reanalyze at GNPS"** text.
 
 **IMAGE**
 
 4. Select the files you wish to include in the reanalysis by clicking the desired group button (*i.e.* G1-G6).
   * The orange buttons in the center of the screen correspond to Sample Information categories.
   
   **IMAGE**
   
   * If filter/s are used, they will appear as red box/boxes in the Attribute Filters Panel (upper-right corner) of the page. To remove already selected filters click on the red boxed filter you wish to remove and the item should disappear from Attribute Filters Panel.
   
   **IMAGE**
   
   * When files are selected into a group the corresponding button becomes red and the number of files is updated in the Selection Summary Panel (upper-left corner).
   
   **IMAGE**
 
 **Example:** The .gif below illustrates the selection of files using a filter based on "human" in Curated_SampleType, and the addition of urine files to group 1 (*i.e.* G1).
     
  **GIF**
 
 5. Click on the **Set up GNPS Networking** button (blue) at the bottom of the page.
 6. Launch the molecular networking job with default parameters or customize parameters. Further documentation on GNPS molecular networking is located [here](https://ccms-ucsd.github.io/GNPSDocumentation/).
 
 ### Notes:
 * You must have an account at [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash2.jsp) and be signed in prior to launching a job.
 * The number of groups is currently limited to 6.
 * The suggested limit for molecular networking is a total of **2500 files**.

# Reanalyze Public Data: GNPS Library Search

 ### Example Use Cases
 * **Annotate chemicals** in the public data via spectral library matching using custom parameters.
 
 ### Summary
A **GNPS library search** has been performed for all files with sample information in GNPS using default parameters. The results are used in the **Chemical Enrichment Analysis** as well as **Sample Information Enrichment Analysis**. This tools allows the user to reanalyze the public data via custom library search parameters. The **library search results** are displayed on GNPS which includes the option of downloading a table with every chemical annotation versus the files it was detected in (cells of the matrix reflect detected, 1, or not detected, 0). Further documentation on GNPS library search is located [here](https://ccms-ucsd.github.io/GNPSDocumentation/).

Chemical annotation is performed in [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash2.jsp) by comparing MS2 spectra, specifically product ion spectra, with reference MS2 fragmentation patterns (GNPS integrates of the majority of public reference MS2 spectra library). GNPS annotations via spectral reference matching are considered level 2 (putative annotation based on spectral library similarity) or 3 (putatively characterized compound class based on spectral similarity to known compounds of a chemical class) by the 2007 metabolomics standard initiative [PMID: 24039616](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3772505/).
 
 ### Tutorial
 1. Log into a [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash2.jsp) account.
 2. Navigate to the [ReDU-MS2](http://dorresteinappshub.ucsd.edu:5005/) homepage.
 3. Click on the **"Select Data to Reanalyze at GNPS"** text.
 
 **IMAGE**
 
 4. Select the files you wish to include in the reanalysis by clicking the **Group 1 (G1)** button.
   * The orange buttons in the center of the screen correspond to Sample Information categories.
   
   **IMAGE**
   
   * If filter/s are used, they will appear as red box/boxes in the Attribute Filters Panel (upper-right corner) of the page. To remove already selected filters click on the red boxed filter you wish to remove and the item should disappear from Attribute Filters Panel.
   
   **IMAGE**
   
   * When files are selected into a group the corresponding button becomes red and the number of files is updated in the Selection Summary Panel (upper-left corner).
   
   **IMAGE**
 
 **Example:** The .gif below illustrates the selection of files using a filter based on "human" in Curated_SampleType, and the addition of urine files to group 1 (*i.e.* G1).
     
  **GIF**
 
 5. Click on the **Set up GNPS Library Search** button (blue) at the bottom of the page.
 6. **Add your data** to **Group 1 (G1)**
 6. Launch the library search job with default parameters or customize parameters. Further documentation on GNPS library search is located [here](https://ccms-ucsd.github.io/GNPSDocumentation/).
 
 ### Notes:
 * You must have an account at [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash2.jsp) and be signed in prior to launching a job.
 * All files must be added to **Group 1 (G1)**; there is no support for multiple groups for library search.
 * The suggested limit for GNPS library search is a total of **5000 files**.

# Reanalyze Public Data: Chemical Enrichment Analysis

### Example Use Cases
* **Explore which chemicals have been detected in *a subset of* the public data** in order to test or develop hypotheses, and determine the specific files in the public data that are relevant for follow up analysis. *viz.* I'm interested in the chemical differences between human urine and human blood - what are they?

### Summary
**All chemical annotations that originate from the selected public data are tabulated by group (G1-G6).** Chemical annotation is performed in [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash2.jsp) by comparing MS2 spectra, specifically product ion spectra, with reference MS2 fragmentation patterns (GNPS integrates of the majority of public reference MS2 spectra library). Default library search parameters are used.

### Tutorial
1. Navigate to the [ReDU-MS2](http://dorresteinappshub.ucsd.edu:5005/) homepage.
2. Click on the **"Select Data to Reanalyze at GNPS"** text.

**IMAGE**

3. Select the files you wish to include in the reanalysis by clicking the desired group button (*i.e.* G1-G6).
   * The orange buttons in the center of the screen correspond to Sample Information categories.
  
  **IMAGE**
  
  * If filter/s are used, they will appear as red box/boxes in the Attribute Filters Panel (upper-right corner) of the page. To remove already selected filters click on the red boxed filter you wish to remove and the item should disappear from Attribute Filters Panel.

  
  **IMAGE**
  
  * When files are selected into a group the corresponding button becomes red and teh number of files is updated in the Selection Summary Panel (upper-left corner).
  
  **IMAGE**

**Example:** The .gif below illustrates the selection of files using a filter based on "human" in Curated_SampleType, and the addition of urine files to group 1 (*i.e.* G1).
    
 **GIF**

4. Click on the **Launch Chemical Enrichment Analysis** button (blue) at the bottom of the page.

**IMAGE**

### Notes:
* GNPS annotations via spectral reference matching are considered level 2 (putative annotation based on spectral library similarity) or 3 (putatively characterized compound class based on spectral similarity to known compounds of a chemical class) by the 2007 metabolomics standard initiative [PMID: 24039616](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3772505/).
* **The same chemical can have multiple GNPS annotations.** Slight variation in the MS2 spectra (*m/z* or abundance) cause the pattern to match different reference MS2 spectra for the same chemical. Users are highly-encouraged to double check their findings.

# Reanalyze Public Data: Sample Information Enrichment Analysis

### Example Use Cases
* **Explore associations between chemcials found in *a subset of* the public data** and sample information in order to test or develop hypotheses. The information could be used to guide follow up analysis using public data that might be relevant.

### Summary
**All chemical annotations that originate from the selected public data are tabulated with a button to view the sample information enrichment for each chemical annotated.** Chemical annotation is performed in [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash2.jsp) by comparing MS2 spectra, specifically product ion spectra, with reference MS2 fragmentation patterns (GNPS integrates of the majority of public reference MS2 spectra library). Default library search parameters are used. Sample information enrichment uses the sample information provided for each files by the community and users of ReDU-MS2.

### Tutorial
1. Navigate to the [ReDU-MS2](http://dorresteinappshub.ucsd.edu:5005/) homepage.
2. Click on the **"Select Data to Reanalyze at GNPS"** text.

**IMAGE**

3. Select the files you wish to include in the reanalysis by clicking the desired group button (*i.e.* G1-G6).
   * The orange buttons in the center of the screen correspond to Sample Information categories.
  
  **IMAGE**
  
  * If filter/s are used, they will appear as red box/boxes in the Attribute Filters Panel (upper-right corner) of the page. To remove already selected filters click on the red boxed filter you wish to remove and the item should disappear from Attribute Filters Panel.
  
  **IMAGE**
  
  * When files are selected into a group the corresponding button becomes red and the number of files is updated in the Selection Summary Panel (upper-left corner).
  
  **IMAGE**

**Example:** The .gif below illustrates the selection of files using a filter based on "human" in Curated_SampleType, and the addition of urine files to group 1 (*i.e.* G1).
    
 **GIF**

4. Click on the **Launch Sample Information Enrichment Analysis** button (blue) at the bottom of the page.

  **IMAGE**

5. Click on the **"View Enrichment"** button (orange) on the right side of the page for the chemical annotation of interest. *KNOWN BUG: the number of files does not update to reflect user selection*

  **IMAGE**

### Notes:
* GNPS annotations via spectral reference matching are considered level 2 (putative annotation based on spectral library similarity) or 3 (putatively characterized compound class based on spectral similarity to known compounds of a chemical class) by the 2007 metabolomics standard initiative [PMID: 24039616](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3772505/).
* **The same chemical can have multiple GNPS annotations.** Slight variation in the MS2 spectra (*m/z* or abundance) cause the pattern to match different reference MS2 spectra for the same chemical. Users are highly-encouraged to double check their findings.
