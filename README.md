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
<b>title.basics.tsv.gz</b>-Contains the following information for titles:<br>
▪tconst(string) -alphanumeric unique identifier of the title<br>
▪titleType(string) –the type/format of the title (e.g. movie, short, tvseries, tvepisode, video, etc)<br>
▪primaryTitle(string) –the more popular title / the title used by the filmmakers on promotional materials at the point of release<br>
▪originalTitle(string) -original title, in the original language<br>
▪isAdult(boolean) -0: non-adult title; 1: adult title<br>
▪startYear(YYYY) –represents the release year of a title. In the case of TV Series, it is the series start year<br>
▪endYear(YYYY) –TV Series end year. ‘\N’ for all other title types<br>
▪runtimeMinutes–primary runtime of the title, in minutes<br>
▪genres (string array) –includes up to three genres associated with the title<br><br><br>
<b>title.crew.tsv.gz</b>–Contains the director and writer information for all the titles in IMDb. Fields include:<br>
▪tconst(string) -alphanumeric unique identifier of the title<br><br>
▪directors (array of nconsts) -director(s) of the given title<br>
▪writers (array of nconsts) –writer(s) of the given title<br><br><br>
<b>title.episode.tsv.gz</b>–Contains the tv episode information. Fields include:<br>
▪tconst(string) -alphanumeric identifier of episode<br>
▪parentTconst(string) -alphanumeric identifier of the parent TV Series<br><br>
▪seasonNumber(integer) –season number the episode belongs to<br>
▪episodeNumber(integer) –episode number of the tconstin the TV series<br><br><br>
<b>title.principals.tsv.gz</>–Contains the principal cast/crew for titles<br><br>
 ▪tconst(string) -alphanumeric unique identifier of the title<br>
 ▪ordering (integer) –a number to uniquely identify rows for a given titleId<br>
 ▪nconst(string) -alphanumeric unique identifier of the name/person<br>
 ▪category (string) -the category of job that person was in<br>
 ▪job (string) -the specific job title if applicable, else '\N'<br>
 ▪characters (string) -the name of the character played if applicable, else '\N'<br><br><br>
<b>title.ratings.tsv.gz</b>–Contains the IMDb rating and votes information for titles<br>
▪tconst(string) -alphanumeric unique identifier of the title<br>
▪averageRating–weighted average of all the individual user ratings<br>
▪numVotes-number of votes the title has received<br>
<b>name.basics.tsv.gz</b>–Contains the following information for names:<br>
▪nconst(string) -alphanumeric unique identifier of the name/person<br>
▪primaryName(string)–name by which the person is most often credited<br>
▪birthYear–in YYYY format<br>
▪deathYear–in YYYY format if applicable, else '\N'<br>
▪primaryProfession(array of strings)–the top-3 professions of the person<br>
▪knownForTitles(array of tconsts) –titles the person is known for<br>
