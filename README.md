# doi-bils-site-data

This repo holds the data file for the doi-bils-site, *issued_dois.json*. This is the only file that has to updated when new DOIs are issued. For each DOI, one or more links has to be defined to the data sets for which the DOI is issued.

## Format

	{
	    "DOIs": {
	        "10.17044/BILS/Xnnnnnnn": {
	            "data_links": [
	                "http://path/to/data/set"
	            ]
	        },
	        "...": {

	        }
	    }
	}

**NB!** The DOIs have to be in UPPERCASE.

## DOI naming scheme
prefix   |   data set type
---------|----------------
G        |   Genomics
GA       |   Genome annotation
MG       |   Metagenomics
P        |   Protein

Note that the DOI has 7 characters in total, i.e. if the prefix is one letter there are 6 digits, and if the prefix has two letters there are 5 digits.