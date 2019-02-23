# How to Contribute New Data and Sample Information for ReDU-MS2

## Preparing Data
Data must be uploaded to GNPS (gnps.used.edu) or MassIVE (massive.ucsd.edu) - a free account is necessary. We encourage the upload of vendor-specific raw data, *e.g.* .raw (Thermo) and .d (Bruker and Agilent), file formats in addition to open-source file formats (.mzXML, .mzML, or .mgf). The data must be made publicaly avaliable. 

Additional details as to which data are compatible with GNPS can be found [here](https://github.com/CCMS-UCSD/GNPSDocumentation/blob/master/docs/isgnpsright.md) as well as how to [convert files](https://github.com/CCMS-UCSD/GNPSDocumentation/blob/master/docs/fileconversion.md) and [upload](https://github.com/CCMS-UCSD/GNPSDocumentation/blob/master/docs/fileupload.md).

## Preparing Sample Information
To add new sample information to your public data at GNPS, you'll need to create a sample information spreadsheet describing each individual mass spectrometry file. This will need to fit into our own sample information template that is entered according to a controlled vocabulary.

Check out this [template](https://docs.google.com/spreadsheets/d/1xEYFvAR6GlB-Gv3OFr2xgnpNhhe6dznn7h0489HIReY/edit?usp=sharing).

Once your have create your own sample information file saved as a tab separated text file based on the template, you can check if the format is valid below with a drag and drop in the [validator](http://dorresteinappshub.ucsd.edu:5005/addmetadata).

Once your sample information has been updated save your file as gnps_metadata.tsv exactly and update your MassIVE dataset with this gnps_metadata.tsv in the supplementary file category. 

All sample information within MassIVE are imported automatically into ReDU-MS2.

# Example
1. Access the [validator](http://dorresteinappshub.ucsd.edu:5005/addmetadata).

**IMAGE HERE**

2. Drag and drop the sample information file (tab separated text file).

**IMAGE HERE**

3. Review the Summary

**IMAGE HERE**

4. A pop-up will indicate if any validation error/s exist. The specific header, line number, and error string of the error/s will be displayed at the bottom of the webpage (limited to the first 500 errors).

**IMAGE HERE**
