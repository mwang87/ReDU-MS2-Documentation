# Frequently Asked Questions (FAQ) by Topic

## General Questions

!!! question "Can I use data in other public data repositories?"
	At present, ReDU only interacts with MassIVE; however, there are plans to incorporate data and metadata from other resources.

!!! question "Can any data be contributed?"
	**Yes!** We accept any data acquired using any extraction method, ionization source (*e.g.* ESI, MALDI, CI, EI, and ambient ionization), pre-MS separation (*e.g.* liquid chromatography, gas chromatography, or capillary electrophoresis) or no separation, mass spectrometer (*e.g.* Orbtrap, QToF, QqQ, LTQ), etc. **However, the data must contain MS/MS data, be converted to an open format, and made public on MassIVE**. Detailed instructions are can be found in the "How to Contribute" section of the documentation - [link here](HowtoContribute.md)

## ReDU Sample Information Validation

!!! question "What are common reasons why validation of my sample information fails?"
	- Values are treated as numbers when the **fill down function is used causing +1 to be added to each row**. Commonly encountered in the MassiveID column and other columns that the spreadsheet program interprets as numeric.
		- **Solution**: update the sample information and revalidate.
	- **Values are not accepted terms.** Accepted terms are displayed in the validation error.
		- **Solution**: If the desired term is not avaliable, please add an issue to GitHub - [link here](https://github.com/mwang87/ReDU-MS2-GNPS).
		
!!! question "I do not see an option in the template?"
	- **Solution**: If the desired term is not avaliable, please add an issue to GitHub - [link here](https://github.com/mwang87/ReDU-MS2-GNPS).

## Molecular Networking or Library Search

!!! question "How do I find out more about molecular networking or library search?"
	please see the documentation at GNPS - [link here](https://ccms-ucsd.github.io/GNPSDocumentation/)

## Emperor Plots

!!! question "How do I find out more about the plotting options in Emperor?"
	please see the GitHub and documentation for Emperor - [link here](https://github.com/biocore/emperor)

---

## Detailed Issues and/or Suggestions
- Please submit any issues or suggestions via [GitHub](https://github.com/mwang87/ReDU-MS2-GNPS).
- The use of the [GNPS forum](https://groups.google.com/forum/#!forum/molecular_networking_bug_reports) is encouraged.
