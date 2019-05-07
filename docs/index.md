# Welcome to the Reanalysis of Data User Interface for MS2 (ReDU-MS2) or "Re-Do"

[ReDU-MS2](http://dorresteinappshub.ucsd.edu:5005/) is a web-based user interface that can be used to easily **Analyze Your Data** or **Analyze Public Data** mass spectrometry data, specifically MS2 (aka tandem mass spectrometry, MS<sup>2</sup>, MS/MS) data. The user interface allows one to select public mass spectrometry files in [MassIVE](https://massive.ucsd.edu/ProteoSAFe/static/massive.jsp), a public mass spectrometry data repository, based on a curated set of sample information and launch reanalyses in the Global Natural Products Social Molecular Networking [GNPS](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash2.jsp) platform.

MS2 data, specifically product ion scans, are obtained from user-submitted open-source data files (.mzXML) and analyzed *de novo* using molecular networking and chemical annotations within GNPS.

**This is a community effort and everyone is encouraged to participate by submitting their own data and sample information ([instructions](HowtoContribute.md)).**

We are developing two main branches of functionality:

## Analyze Your Data
* [Compare Your Data to Public Data via Multivariate Analysis](AnalyzeYourData_MultivariateComparisons.md) - Projection of your data onto a precalculated principal components analysis score plot of public data. <br>
* [Co-analyze Your Data with Public Data at GNPS](AnalyzeYourData_CoAnalysis_at_GNPS.md) - Select files using sample information and assemble public data in groups as desired using the file selector. Launching an analysis loads the files from MassIVE at which point users can add their own data. The following co-analyses can be launched:
  * Molecular Networking at GNPS
  * Library Search at GNPS
  * Chemical Enrichment Analysis

## Analyze Public Data
* [Explore Multivariate Analysis of Public Data](AnalyzePublicData_MultivariateComparisons.md) - Explore precalculated principal components analysis score plot of public data. <br>
* [Explore Chemical Annotations and Associated Sample Information in all Public Data](AnalyzePublicData_ChemicalEnrichment.md) - Precalculated using public data and default GNPS parameters <br>
* [Re-analyze Public Data at GNPS](PublicData_Reanalysis_at_GNPS.md) - Select files using sample information and assemble public data in groups as desired using the file selector. The following co-analyses can be launched:
  * Molecular Networking at GNPS
  * Library Search at GNPS
  * Chemical Enrichment Analysis
 
## Data and Code Availability ##
* All sample information can be downloaded from the ReDU-MS2 homepage by clicking "Download Database".
* The data processed for the chemical and sample information enrichment analysis can be downloaded using an accomanying Jupyter Notebook (**link here**).
* Table generated in the user-interface can be downloaded using an accomanying Juypter Notebook (**link here**).

**anyone who creates custom code is encouraged it to share with the rest of ReDU-MS2 users**
