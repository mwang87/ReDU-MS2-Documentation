# Welcome to ReDU :)
## Reanalysis of Data User Interface

[ReDU](https://redu.ucsd.edu/) is a community- and data-driven approach to find and reuse public data containing tandem MS data at the repository scale. ReDU is a launchpad for co- or re-analysis of public data via the Global Natural Product Social Molecular Networking Platform [(GNPS)](https://gnps.ucsd.edu/ProteoSAFe/static/gnps-splash.jsp). Our aim is to empower researchers to put their data in the context of public data as well as explore questions using public data at the repository scale.

**This is a community effort and everyone is encouraged to participate by submitting their own data and sample information [instructions](HowtoContribute.md). The sharing of new applications (and code) which use ReDU is highly encouraged.**

```mermaid
	graph LR
		subgraph 
		A1["File Selection Interface"]
		A2["Set Up Co-Analysis with GNPS Molecular Networking"]
		A3["Set Up Co-Analysis with GNPS Library Search"]
		A4["Launch Group Comparator"]
		A5["Launch Chemical Explorer"]
		A6["Launch PCA of Selected Files"]
		
		A1 --> A2
		A1 --> A3
		A1 --> A4
		A1 --> A5
		A1 --> A6
		end
		
		subgraph 
		B1["Chemical Explorer"]
		B2["View Files"]
		B3["View Associations"]
		
		B1 --> B2
		B1 --> B3
		A5 --> B1
		click B1 "https://redu.ucsd.edu/compoundslist" "Link Out Chemical Explorer"
		end

		subgraph 
		C1["Analyze Public Data"]
		C2["Explore Multivariate Analysis of Public Data"]
		C3["Chemical Explorer"]
		C4["Re-analyze Public Data at GNPS"]
		
		C1 --> C2
		C1 --> C3
		C1 --> C4
		
		C4 --> A1
		C1 --> B1
		end
		
		subgraph 
		D1["Analyze Your Data"]
		D2["Compare Your Data to Public Data via Multivariate Analysis"]
		D3["Co-analyze Your Data with Public Data at GNPS"]

		D1 --> D2
		D1 --> D3

		D3 --> A1
		end
		subgraph 
		E1["GNPS"]
		E2["GNPS Molecular Networking Interface"]
		E3["GNPS Library Search Interface"]
		
		E1 --> E2
		E1 --> E3

		A2 --> E1
		A3 --> E1
		end
```
## We are developing two main branches of functionality:

## Analyze Your Data
* [Compare Your Data to Public Data via Multivariate Analysis](AnalyzeYourData_MultivariateComparisons.md) - Projection of your data onto a precalculated principal components analysis score plot of public data. <br>
* [Co-analyze Your Data with Public Data at GNPS](AnalyzeYourData_CoAnalysis_at_GNPS.md) - Select files using sample information and assemble public data in groups as desired using the file selector. Launching an analysis loads the files from [MassIVE](https://massive.ucsd.edu/ProteoSAFe/static/massive.jsp) at which point users can add their own data. The following co-analyses can be launched:
  * Molecular Networking at GNPS
  * Library Search at GNPS
  
## Analyze Public Data
* [Explore Multivariate Analysis of Public Data](AnalyzePublicData_MultivariateComparisons.md) - Explore precalculated principal components analysis score plot of public data. <br>
* [Explore Chemical Annotations and Associated Sample Information in all Public Data](AnalyzePublicData_ChemicalExplorerSampleInformationAssociation.md) - Precalculated using public data and default GNPS parameters <br>
* [Re-analyze Public Data at GNPS](PublicData_Reanalysis_at_GNPS.md) - Select files using sample information and assemble public data in groups as desired using the file selector. The following co-analyses can be launched:
  * Molecular Networking at GNPS
  * Library Search at GNPS
  * Chemical Enrichment Analysis
  * Sample Information Association
 
## Data Availability
All sample information can be downloaded from the ReDU-MS2 homepage by clicking "Download Database". The ReDU identification database is publicly available and accessible via GNPS/MassIVE (gnps.ucsd.edu), MSV000084206.
