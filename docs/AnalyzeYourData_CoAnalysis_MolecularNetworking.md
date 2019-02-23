# Analyze Your Data: Co-Analyze your Data via GNPS Molecular Networking

## Example Use Cases
* **Annotate unknown chemicals** in your data by linking it to annotated chemicals in public data from the same sample type (*e.g.* human urine)
* **Enhanced context** of chemicals detected in your own data, *e.g.* (bio)chemical transformations, by comparing chemicals detected in public data from the same sample type (*e.g.* human urine)

## Summary
[Molecular Networking](https://www.nature.com/articles/nbt.3597?WT.ec_id=NBT-201608&spMailingID=52025126&spUserID=ODkwMTM2NjI1NQS2&spJobID=981583612&spReportId=OTgxNTgzNjEyS0) is performed in GNPS. Users can co-analyze their data with public data by selecting files using a simple file selector. The file selector allows one to select (and filter) files based on the sample information provided with every file, and place multiple types of files into one of 6 different groups (*i.e.* G1-G6). A single button click on "Set up GNPS Networking" loads all the files and launches a GNPS molecular job; an email will be sent when the job has finished. Further documentation on GNPS molecular networking is located [here](https://ccms-ucsd.github.io/GNPSDocumentation/).

## Tutorial
1. Log into a [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash2.jsp) account.
2. Navigate to the [ReDU-MS2](http://dorresteinappshub.ucsd.edu:5005/) homepage.
3. Click on the **"Select Data to Co-Analyze"** text.

**IMAGE**

4. Select the files you wish to include in the co-analysis by clicking the desired group button (*i.e.* G1-G6).
  * The orange buttons in the center of the screen correspond to Sample Information categories.
  
  **IMAGE**
  
  * If filter/s are used, they will appear as red boxed in the Attribute Filters Panel (upper-right corner) of the page.
  
  **IMAGE**
  
  * When files are selected into a group the corresponding button becomes red and teh number of files is updated in the Selection Summary Panel (upper-left corner).
  
  **IMAGE**

**Example:** The .gif below illustrates the selection of files using a filter based on "human" in Curated_SampleType, and the addition of urine files to group 1 (*i.e.* G1).
    
 **GIF**

5. Click on the **Set up GNPS Networking** button (blue) at the bottom of the page.
6. **Add your data** to one of the remaining groups (*i.e.* G1-G6).
6. Launch the molecular networking jobs with default parameters or customize parameters. Further documentation on GNPS molecular networking is located [here](https://ccms-ucsd.github.io/GNPSDocumentation/).

## Notes:
* You must have an account at [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash2.jsp) and be signed in prior to launching a job.
* The number of groups is currently limited to 6.
* The suggested limit for molecular networking is a total of **2500 files**.
