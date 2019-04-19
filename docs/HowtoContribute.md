# How to Contribute New Data and Sample Information for ReDU-MS2

## Preparing Data
Data must be uploaded to GNPS (gnps.used.edu) or MassIVE (massive.ucsd.edu) - a free account is necessary - into a new MassIVE ID. We encourage the upload of vendor-specific raw data, *e.g.* .raw (Thermo) and .d (Bruker and Agilent), file formats in addition to open-source file formats (.mzXML, .mzML, or .mgf). After completetion of the initial workflow to create the MassIVE ID, please click the "make public" and "convert spectra" buttons.

Additional details as to which data are compatible with GNPS can be found [here](https://github.com/CCMS-UCSD/GNPSDocumentation/blob/master/docs/isgnpsright.md) as well as how to [convert files](https://github.com/CCMS-UCSD/GNPSDocumentation/blob/master/docs/fileconversion.md) and [upload](https://github.com/CCMS-UCSD/GNPSDocumentation/blob/master/docs/fileupload.md).

## Preparing Sample Information
Sample information is synonymous with file-level metadata, and it is necessary for data to be included in ReDU-MS2. One sample information file is required <b>per MassIVE ID</b> (it can contain multiple sample types, experiments, etc), and should be uploaded to the same MassIVE ID as the data. <br>

The file is required to adhere to the template which uses a controlled vocabulary. <b>If you require options that are not avaliable in the template, please contact the admins (<b>contact page hyperlink</b>) in order to update the options.</b> Note, sample information that does not adhere to the controlled vocabulary will be removed on a file-by-file basis. <br>

To add new sample information to your public data at GNPS, you'll need to create a sample information spreadsheet describing each individual mass spectrometry file. This will need to fit into our own sample information template that is entered according to a controlled vocabulary. <br>

The sample information template can be found [here](https://docs.google.com/spreadsheets/d/1xEYFvAR6GlB-Gv3OFr2xgnpNhhe6dznn7h0489HIReY/edit?usp=sharing).<br>

<b>The sample information file can be created by completing the following steps.</b><br>
1. Users should save a copy of the sample information template by going to "File - Make a copy" into their personal google drive.
2. Users can then fill in sample information using drop-downs when applicable (grey columns are automatically entered using formulae). If copying and pasting, please copy+special and paste without changing the cell formulae. The accepted entries when vocublary is controlled is displayed, per column, in "TheMagic" tab. <b>If you require options that are not avaliable in the template, please contact the admins</b>
3. When completed, delete all extra rows. Download from Google Sheets as a tab separated text file by "File-Download as" and selecting "Tab-seperated values..."
4. Rename the file as <b> gnps_metadata.tsv" </b> (it must be this exact name).
5. Check the sample informatoin using the drag-and-drop <b> validator </b> [validator](http://dorresteinappshub.ucsd.edu:5005/addmetadata). The validator will indicate via a message if there are any errors. Non-adherant information is displayed in the "Sample Information Validation Errors" panel - the row, column, and the accepted terms are listed.
6. Once your sample information has passed validation, upload your sample information file ("gnps_metadata.tsv") to MassIVE (massive.ucsd.edu) by updating the appropriate MassIVE ID. <b>In order to update a MassIVE ID</b>, click the "add files" button in MassIVE and upload the sample information file in the <b>"supplementary file"</b> option. 
 
<b>Notes:</b> Sample information files are automatically imported into ReDU-MS2 multiple times per day from MassIVE. Any conflict between identically named files will result in their exclusion. The filename present in the same folder must match the uploaded data (.mzML or .mzXML). If corrections or updates are necessary, please make them accordingly and upload the new sample information file - our system will automatically import the most recent version of the "gnps_metadata.tsv" file (files cannot be deleted by users from MassIVE).
  
# Example
1. Access the [validator](http://dorresteinappshub.ucsd.edu:5005/addmetadata).

**IMAGE HERE**

2. Drag and drop the sample information file (tab separated text file).

**IMAGE HERE**

3. Review the Summary

**IMAGE HERE**

4. A pop-up will indicate if any validation error/s exist. The specific header, line number, and error string of the error/s will be displayed at the bottom of the webpage (limited to the first 500 errors).

**IMAGE HERE**
