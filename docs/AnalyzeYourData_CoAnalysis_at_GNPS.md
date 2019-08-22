# Analyze Your Data: Co-analyze Your Data with Public Data at GNPS

2 data analysis options currently supported in ReDU (details below in the corresponding section):
* Molecular Networking at GNPS
* Library Search at GNPS <br>

## Molecular Networking at GNPS

### Example Use Cases
* **Annotate unknown chemicals in your samples** Molecular networking links chemicals based on MS/MS spectra similarity. Files across data sets from the same sample type can be selected easily and included with your own data. One can find annotations that enhance the context of your own data by including public data.

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
 5. Click on the **Set Up Co-Analysis with GNPS Networking** button (blue) at the bottom of the page.
 6. **Add your data** to one of the remaining groups (*i.e.* G1-G6).
 7. Launch the molecular networking job with default parameters or customize parameters. Further documentation on GNPS molecular networking is located [here](https://ccms-ucsd.github.io/GNPSDocumentation/).

![File Selector](images/File_Selector.gif)

### Notes:
 * You must have an account at [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash.jsp) and be signed in prior to launching a job.
 * The number of groups is currently limited to 6.
 * The suggested limit for molecular networking is a total of **3000 files**.


## Library Search at GNPS

### Example Use Cases
* **Annotate chemicals in your data as well as public data**  via spectral library matching using custom parameters. Used for generating a list of annotations based on custom parameters for your files and public files included for further analysis. All files must be in G1.

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
 5. Click on the **Set Up Co-Analysis with GNPS Library Search** button (blue) at the bottom of the page.
 6. **Add your data** to **Group 1 (G1)**
 7. Launch the library search job with default parameters or customize parameters. Further documentation on GNPS library search is located [here](https://ccms-ucsd.github.io/GNPSDocumentation/).

## Notes:
 * You must have an account at [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash.jsp) and be signed in prior to launching a job.
 * All files must be added to **Group 1 (G1)**; there is no support for multiple groups for library search.
 * The suggested limit for GNPS library search is a total of **5000 files**.
