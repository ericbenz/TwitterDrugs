# TwitterDrugs
The TwitterDrugs corpus is a collection of publically available tweets that were mined from 26 January to 22 February 2016. All tweets originally returned by the search API screened automatically for relevancy, resulting in a loss of over 75% of the originally mined data.

The `relevant.ids` file contains tweet IDs, user IDs, and the drug that was used to identify that tweet for relevance. The drugs are listed in the `drugs.txt` file.

The tweet content can be downloaded with the `download_tweets.py` file, released by Azadeh Nikfarjam (Arizona State University) as a compontent of her research group's 2015 work *Pharmacovigilance from social media: mining adverse drug reaction mentions using sequence labeling with word embedding cluster features*. The script requires BeautifulSoup.

## Drugs
The 334 drugs in the `drugs.txt` file represent the 81 drugs present in ADR tweets from the Nikfarjam 2015 study (available [here](http://diego.asu.edu/downloads/publications/ADRMine/drug_names.txt)), the New York State Department of Health [top 150 drugs](https://apps.health.ny.gov/pdpw/DrugInfo/DrugInfo.action) list, and Chemical and Engineering News' [2014 top 50 drugs list](http://cen.acs.org/content/dam/cen/supplements/CEN-supplement092014.pdf).

## Use
This corpus is freely available to the academic community. By downloading Twitter data, you agree to follow the current [Twitter terms of service](https://twitter.com/tos), which requires not to redistribute the tweet content and to delete tweets that are marked deleted in the future.

## Contact
Please email `ericbenz` at `brandeis` dot `edu` with questions or concerns.
