# curatedMetagenomicData 1.19.4

* move functions from data-raw into R
* add folder-selecting functions and parameters to eliminate assumption
of writing within the package source folders

the software seems to be

[1] "cmdValidVersions"           "combined_metadata"         
[3] "curatedMetagenomicData"     "ExpressionSet2MRexperiment"
[5] "ExpressionSet2phyloseq"     "getMetaphlanTree"          
[7] "mergeData"   

# curatedMetagenomicData 1.16.0

* curatedMetagenomicData now contains 10,199 samples from 57 studies
* A total of 2,209 samples added since Bioconductor 3.9 (April 2019)
* Datasets added since Bioconductor 3.9 (April 2019):
    - DhakanDB_2019 (110 samples)
    - GopalakrishnanV_2018 (25 samples)
    - HansenLBS_2018 (208 samples)
    - JieZ_2017 (385 samples)
    - KieserS_2018 (27 samples)
    - MatsonV_2018 (39 samples)
    - PehrssonE_2016 (191 samples)
    - TettAJ_2019_a (68 samples)
    - TettAJ_2019_b (44 samples)
    - TettAJ_2019_c (50 samples)
    - YeZ_2018 (65 samples)
    - ZeeviD_2015 (900 samples)

# curatedMetagenomicData 1.14.0

* curatedMetagenomicData now contains 8,087 samples from 45 studies
* A total of 935 samples added since Bioconductor 3.8 (October 2018)
* Datasets added since Bioconductor 3.8 (October 2018):
    - BackhedF_2015 (381 samples)
    - CosteaPI_2017 (279 samples)
    - FerrettiP_2018 (215 samples)
    - ThomasAM_2018b (60 samples)
* Fixed an error in the metadata for HMP_2012 where posterior fornix samples were incorrectly tagged as 'oralcavity'
* Removed metadata from HMP_2012 attributing the study to Federal Urdu University... Karachi, Pakistan
* WenC_2017 has been renamed ChengpingW_2017
* WenC_2017 is deprecated and will be removed in the next release

# curatedMetagenomicData 1.12.0

* curatedMetagenomicData now contains 7,152 samples from 41 studies
* A total of 766 samples added since Bioconductor 3.7 (May 2018) relaese
* Datasets added since Bioconductor 3.7 (May 2018) release:
    - Bengtsson-PalmeJ_2015 (70 samples)
    - DavidLA_2015 (49 samples)
    - KosticAD_2015 (124 samples)
    - LiSS_2016 (55 samples)
    - LoombaR_2017 (86 samples)
    - OlmMR_2017 (45 samples)
    - PasolliE_2018 (112 samples)
    - ShiB_2015 (48 samples)
    - ThomasAM_2018a (80 samples)
    - WenC_2017 (97 samples)
* Fixed a bug in expressionset names where "-"s would be replaced with "_"
* As a result of this fix, the following datasets are deprecated and will be removed in the next release:
    - Bengtsson_PalmeJ_2015
    - Castro_NallarE_2015
    - Heitz_BuschartA_2016
    - Obregon_TitoAJ_2015

# curatedMetagenomicData 1.10.0

* curatedMetagenomicData now contains 6386 samples from 31 studies : )
* A total of 328 samples added since Bioconductor 3.6 (October, 2017) release
* Datasets added since Bioconductor 3.6 (October, 2017) release
    - LiJ_2017 (196 samples)
    - LouisS_2016 (92 samples)
    - SmitsSA_2017 (40 samples)
* A curator field has been added to metadata to credit the work of curators
* curatedMetagenomicData is currently on a diet and being refactored:
    - The docs directory used to build the github pages site has been moved to a
      branch, making the R package smaller
    - All code used for processing of raw data in R is moving to a seperate
      GitHub repository curatedMetagenomicDataPipeline
    - Curation takes place in the curatedMetagenomicDataCuration repository and
      curation is automatically checked; contributions are welcomed
    - All code used for processing of raw data beyond R is moving to a seperate
      GitHub repository curatedMetagenomicDataHighLoad
* All data has been reprocessed to ensure updated and correct curation

# curatedMetagenomicData 1.8.0

* curatedMetagenomicData now contains 6058 samples from 28 studies : )
* A total of 3,152 samples added since Bioconductor 3.5 (April, 2017) release
* Datasets added since Bioconductor 3.5 (April, 2017) release
    - HanniganGD_2017 (82 samples)
    - LiJ_2014 (260 samples)
    - AsnicarF_2017 (26 samples)
    - BritoIL_2016 (312 samples)
    - Castro-NallarE_2015 (32 samples)
    - ChngKR_2016 (78 samples)
    - FengQ_2015 (154 samples)
    - Heitz-BuschartA_2016 (53 samples)
    - LiuW_2016 (110 samples)
    - RaymondF_2016 (72 samples)
    - SchirmerM_2016 (471 samples)
    - VatanenT_2016 (785 samples)
    - VincentC_2016 (229 samples)
    - VogtmannE_2016 (110 samples)
    - XieH_2016 (250 samples)
    - YuJ_2015 (128 samples)
* The cmdversion argument was removed from the curatedMetagenomicData() function
* Calls to curatedMetagenomicData() simply return the newest version of the data
* Older versions of datasets are accessible by using the named functions
* Added phylogenetictree = TRUE argument to ExpressionSet2phyloseq()

# curatedMetagenomicData 1.6.0

* doubled the number of samples to over 5,700
* made naming of metadata more complete and strict, see inst/extdata/template.csv
* mergeData() function for convenient merging of datasets
* combined_metadata table providing all sample information for all studies

# curatedMetagenomicData 1.4.0

* Data updated to include accession numbers
* Minor updates to PaperFigures.Rmd vignette for reproducibility

# curatedMetagenomicData 1.2.0

* Vast improvements to documentation, now more informative and compact
* New function to coerce data to an MRexperiment class
* New workhorse function to access data with wildcard search
* Fun intro message for developers
* Fixed a bug related to ExperimentHub that caused checks to fail

# curatedMetagenomicData 1.0.4

* Fixed a bug related to ExperimentHub that caused checks to fail

# curatedMetagenomicData 1.0.0

* Package vignette is updated to reflect in the intended use of ExperimentHub
* Object level documentation is update for completeness and aliased
* Minor description file changes to ensure collation order
* Version bumped to reflect latest y version of Bioconductor
* All data is reprocessed in R (v3.3.2)

# curatedMetagenomicData 0.99.8

* Codebase is completely refactored to ExperimentHub specifications
* Package vignette is updated to Rmd syntax and uses BiocStyle
* New parallel functions allow for faster data processing
* Documentation updated to use roxygen2
* All data is reprocessed in R (v3.3.1)
* All raw data is reprocessed with MetaPhlAn2 (v2.2.0) & HUMAnN2 (v0.7.0)
