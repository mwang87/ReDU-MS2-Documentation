# How to Contribute New Data and Sample Information for ReDU-MS2

## [Instructions](http://dorresteinappshub.ucsd.edu:5005/addmetadata)
## [Sample Information Template](https://docs.google.com/spreadsheets/d/1v71bnUd8fiXX51zuZIUAvYETWmpwFQj-M3mu4CNsHBU/edit?usp=sharing)

## Additional Details
### Preparing Data
Data must be uploaded to GNPS (gnps.used.edu) or MassIVE (massive.ucsd.edu) - a free account is necessary. We encourage the upload of vendor-specific raw data, *e.g.* .raw (Thermo) and .d (Bruker and Agilent), file formats in addition to open-source file formats (.mzXML, .mzML, or .mgf). The data must be made publicly avaliable. 

Additional details as to which data are compatible with GNPS can be found [here](https://github.com/CCMS-UCSD/GNPSDocumentation/blob/master/docs/isgnpsright.md) as well as how to [convert files](https://github.com/CCMS-UCSD/GNPSDocumentation/blob/master/docs/fileconversion.md) and [upload](https://github.com/CCMS-UCSD/GNPSDocumentation/blob/master/docs/fileupload.md).

### What is Sample Information in ReDU-MS2?
Sample information is synonymous with file-level metadata, and it is necessary for data to be included in ReDU-MS2. One sample information file is required per MassIVE ID (it can contain multiple sample types, experiments, etc), and should be uploaded to the same MassIVE ID as the data. The file is required to adhere to the template which uses a controlled vocabulary. If you require options that are not avaliable in the template, please raise an issue on [GitHub](https://github.com/mwang87/ReDU-MS2-GNPS) in order to update the options. Note, sample information that does not adhere to the controlled vocabulary will be removed on a file-by-file basis.

### The sample information file can be created by completing the following steps.
* Save a copy of the sample information template by going to "File - Make a copy" into a personal google drive.<br>
**IMAGE HERE**

* Fill in sample information using drop-downs when applicable (grey columns at the end of the template are automatically entered using formulae). If copying and pasting, please copy+special and paste without changing the cell formulae. The accepted options in the controlled vocublary is indicated, per column, in "ReDUMS2_controlled_vocabulary" tab. If you require options that are not avaliable, please raise an issue on [GitHub](https://github.com/mwang87/ReDU-MS2-GNPS).<br>
**IMAGE HERE**

* When completed, delete all extra rows of the template. Download from Google Sheets as a tab separated text file using "File-Download as" and selecting "Tab-seperated values..."<br>
**IMAGE HERE**

* Rename the file as gnps_metadata.tsv" (it must be this exact name and file extension).<br>
**IMAGE HERE**

* Check the sample informatoin using the drag-and-drop validator below. The validator will indicate via a message if there are any errors. Non-adherant information is displayed in the "Sample Information Validation Errors" panel - the row, column, and the accepted terms are listed. <br>
**IMAGE HERE**

* If errors occur please make the appropriate changes in the sample information template and repeat the renaming and validation steps. When no errors occur and validation passes, upload your sample information file ("gnps_metadata.tsv") to MassIVE (massive.ucsd.edu) by updating the appropriate MassIVE ID. In order to update a MassIVE ID, click the "add files" button in MassIVE and upload the sample information file in the "supplementary file" option.<br>
**IMAGE HERE**

### Notes
Sample information files are automatically imported into ReDU-MS2 multiple times per day from MassIVE. Any conflict between identically named files will result in their exclusion. The filename present in the same folder must match the uploaded data (.mzML or .mzXML). If corrections or updates are necessary, please make them accordingly and upload the new sample information file - our system will automatically import the most recent version of the "gnps_metadata.tsv" file (files cannot be deleted by users from MassIVE).
