# AGNES Case Study Data

The [assessed-result-set.csv](assessed-result-set.csv)
 file contains all the results from the following queries in the [AGNES](http://agnes.liacs.nl/search/agnesv2) system:

|Start Year|End Year|Free Text Query|
| -------- | -------|---------------|
|450|900|crematie|
|450|900|crematie*|
|450|900|verbrand menselijk bot|
|450|900|brandstapel|
|450|900|brandstapel*|
|450|900|urn|
|450|900|knochenlager|
|450|900|beendernest|
|450|900|brandgrube|

Below you can find the code table explaining all the headers (line 1 of the CSV file):

|Field Name|Description|Notes|
| -------- | ----------|-----|
|title|Title of the document||
|authors|Authors of the document|Separated by semi-colon (;)|
|file_type|The type of document||
|page_numbers|Which pages contain the search terms|Separated by slash (/)|
|subjects|Subject metadata from DANS||
|locations|Location metadata from DANS||
|doi|DOI||
|archis_number|Case number in the Archis system||
|lat|Latitude in WGS84||
|lon|Longitude in WGS84||
|description|Description of file, as per DATA metadata||
|relevant|Relevancy|0 = not relevant, 1 = moderately relevant, 2 = very relevant|
|known|Whether the file was known to experts|0 = no, 1 = yes|

The last 7 columns represent each query, and if the document occurs in the result set for that query, it is marked with 1, otherwise with 0.

The definitions of 0, 1 and 2 in the 'relevant' column are defined as follows:

0: completely irrelevant (no Early Medieval cremation)
1: moderately relevant (reference to other file, or either the cremation or the date is not certain)
2: very relevant (clearly an Early Medieval cremation)

