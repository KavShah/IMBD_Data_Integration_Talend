# IMBD_DataIntegration_Talend
## IMDb Datasets
IMDb Dataset DetailsEach dataset is contained in a gzipped, tab-separated-values (TSV) formatted file in the UTF-8 character set. The first line in each file contains headers that describe what is in each column. A‘\N’is used to denote that a particular field is missing or null for that title/name. The available datasets are as follows:<br>
•title.akas.tsv.gz-Contains information for titles.<br>
•title.basics.tsv.gz-Contains information for titles.<br>
•title.crew.tsv.gz–Contains the director and writer information for all the titles in IMDb. <br>
•title.episode.tsv.gz–Contains the tv episode information.<br>
•title.principals.tsv.gz–Contains the principal cast/crew for titles<br>
•title.ratings.tsv.gz–Contains the IMDb rating and votes information for titles<br>
•name.basics.tsv.gz–Contains information for names.<br><br><br>
<b>title.akas.tsv.gz</b>-Contains the following information for titles:<br>
▪titleId(string) -a tconst, an alphanumeric unique identifier of the title<br>
▪ordering (integer) –a number to uniquely identify rows for a given titleId<br>
▪title (string) –the localized title<br>
▪region (string) -the region for this version of the title<br>
▪language (string) -the language of the title<br>
▪types (array) -Enumerated set of attributes for this alternative title. One or more of the following: "alternative", "dvd", "festival", "tv", "video", "working", "original", "imdbDisplay". New values may be added in the future without warning<br>
▪attributes (array) -Additional terms to describe this alternative title, not enumerated<br><br><br>
