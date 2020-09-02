# How to Contribute to ReDU

!!! info "Required Items"
	1. **A free MassIVE account is required to contribute data and a free GNPS account is required to analyze data.**
		- Please sign-up at the MassIVE homepage - [link here](https://massive.ucsd.edu/ProteoSAFe/static/massive.jsp)
		- Please sign-up at the GNPS homepage - [link here](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash.jsp)
	2. **Mass spectrometry data (MS/MS data)**
		- Data converted to open-format (.mzXML or .mzML)
		- Data uploaded to MassIVE [link here](https://massive.ucsd.edu/ProteoSAFe/static/massive.jsp) as a public dataset
	3. **ReDU-compliant sample information**
		- Manual completion of the **ReDU sample information template** ([link here](https://docs.google.com/spreadsheets/d/1v71bnUd8fiXX51zuZIUAvYETWmpwFQj-M3mu4CNsHBU/edit?usp=sharing))
		- Validation of the ReDU sample information template using the drag-and-drop validator [link here](https://redu.ucsd.edu/ReDUValidator)
		- Upload ReDU-compliant sample information (after validation) to the corresponding MassIVE accession

---

# Detailed Step-by-step Instructions

## 1. Sign-up for a free MassIVE and GNPS account
- Please sign-up at the MassIVE homepage - [link here](https://massive.ucsd.edu/ProteoSAFe/static/massive.jsp)
- Please sign-up at the GNPS homepage - [link here](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash.jsp)

## 2. Mass spectrometry data (MS/MS data)

### 2.1 Convert mass spectrometry data to open-source file formats
- convert your data to open-source file format accepted in MassIVE

??? info "links to info on data conversion"
    - Instructions on file conversion software - [link here](https://github.com/CCMS-UCSD/GNPSDocumentation/blob/master/docs/fileconversion.md)
    - Information on accepted open-source files formats - [link here](https://github.com/CCMS-UCSD/GNPSDocumentation/blob/master/docs/isgnpsright.md)

### 2.2 Upload mass spectrometry data to GNPS/MassIVE and create a MassIVE ID
- Launch the "Submit your data" workflow to submit your data to MassIVE - [link here](https://massive.ucsd.edu/ProteoSAFe/static/massive.jsp?redirect=auth)) - to create a MassIVE ID. **The title must beginning with "GNPS"**
- You will receive an email when the workflow has completed.
- After complete, make the MassIVE ID public by clicking the **"make public"** button.
- Please click the **"convert spectra"** button to expedite inclusion in ReDU.

??? info "links to info on uploading data and making datasets in MassIVE"
    - Information on making datasets in MassIVE - [link here](https://ccms-ucsd.github.io/GNPSDocumentation/datasets/)
	- Suggested FTP clients - [link here](https://ccms-ucsd.github.io/GNPSDocumentation/fileupload/)
	- We encourage the upload of vendor-specific raw data, *e.g.* .raw (Thermo) and .d (Bruker and Agilent), in addition to open-source file formats (.mzXML, .mzML, or .mgf). <br>

## 3. **ReDU-compliant sample information**

### 3.1 Manual completion of the ReDU sample information template
- Navigate to the ReDU Sample Information Template - [link here](https://docs.google.com/spreadsheets/d/1v71bnUd8fiXX51zuZIUAvYETWmpwFQj-M3mu4CNsHBU/edit?usp=sharing)
- Save a copy of the sample information template by going to **"File - Make a copy"** into a personal google drive

???+ example "how to make a copy of the sample information template - .gif"
	![Make a copy of the template](images/Sample_Template_MakeACopy.gif)

- Fill in sample information using drop-downs when applicable (grey columns at the end of the template are automatically entered using formulae).

???+ example "filling in the sample information template - .gif"
	![Fill in information](images/Sample_Template_Fill.gif)

!!! notes "notes on using the sample information template"
	- One template is required per MassIVE ID
	- It is highly recommended to fill the template in Google Sheets
	- ReDU uses a controlled vocabulary - the accepted terms are listed in the "ReDUMS2_controlled_vocabulary" tab per column. **If you require terms that are not avaliable, please raise an issue on GitHub - [link here](https://github.com/mwang87/ReDU-MS2-GNPS).**
	- Please note that the abbreviation within the metadata "ML import: not available" is for data imported from [MetaboLights](https://www.ebi.ac.uk/metabolights/). We automatically import this data, and sometimes are unable to import metadata categories properly with the controlled vocabulary used in ReDU
	- Columns and values are defined on the readme tab in the template.
	- The filename in the sample information file must match the data uploaded to MassIVE (.mzML or .mzXML). Any conflict between identically named files will result in their exclusion.
	- When copying and pasting from another spreadsheet, please **copy + special paste** so as to not chance the cell formulae or formatting.

### 3.2 Validation of the ReDU sample information template using the drag-and-drop validator
- When complete, **delete all extra rows** of the template
- Download from Google Sheets as a tab separated text file using **"File-Download as" and selecting "Tab-seperated values..."**

???+ example "how to download the sample information template"
	![Delete extra rows in the template](images/Sample_Template_deleterows.gif)

- Navigate to the ReDU Sample Information Validator - [link here](https://redu.ucsd.edu/ReDUValidator)
- Drag-and-drop or select your sample information file into the validator.
	- A message will indicate if the files passes or not.
	- Non-adherant information is displayed in the "Sample Information Validation Errors" panel - the row, column, and the accepted terms are listed.
	- If errors occur, then please correct the non-adherant information in the template and repeat from 2C

???+ example "how to validate the sample information template"
	![Validate the Template](images/Validate.gif)

- Upon passing the validator, **rename the file** to be exactly **"gnps_metadata.tsv"**

!!! warning
	The filename must be **gnps_metadata.tsv** - this step is critical. This is how we find things in the MassIVE repository!

!!! notes "notes on validator use"
	- If corrections or updates are necessary, please make them accordingly and upload the new validated sample information file named **"gnps_metadata.tsv"**. ReDU will automatically import the most recent version of the "gnps_metadata.tsv" file (files cannot be deleted by users from MassIVE).
	- It is suggested to make a seperate directory on your computer to store each MassIVE IDs sample information template.

### 3.3 Upload ReDU-compliant sample information (after validation) to the corresponding MassIVE accession
- Navigate to the MassIVE ID created and click on the **"add files"** button.
- Use the Drag-and-Drop upload option to add the validated sample information file named "gnps_metadata.tsv"
- Select the validated sample information file (named exactly **"gnps_metadata.tsv"**) into the **"Metadata file"** folder *or* **"Supplementary file"** folder
- Submit the update

!!! check "check that your data made it into ReDU"
	- Navigate to ReDU - [link here](https://redu.ucsd.edu/metadataselection)
	- Selecting the "DatasetAccession" button which will load all MassIVE accessions avaliable in ReDU
	- Check for your MassIVE accession (*i.e.* MassIVE ID) and confirm the number of files is correct
	- **Note: GNPS/MassIVE is searched multiple times per day to find new or updated sample information files so it may take some time for your data to appear.**

!!! Success
	Congrats and thank you for contributing to ReDU! :thumbsup:

# Help and Advice
- General Questions or Advice = GNPS Forum - [link here](https://groups.google.com/forum/#!forum/molecular_networking_bug_reports) <br>
- New Terms, Corrections, Suggestions = GitHub - [link here](https://github.com/mwang87/ReDU-MS2-GNPS)
