# TwitterDrugs
The TwitterDrugs corpus is a collection of 166,551 publically available tweets that were mined from 26 January to 26 February 2016, containing over 2.5 million tokens. Approximately 780,000 tweets were originally returned by the Twitter search API before being screened for relevancy for final inclusion, resulting in a loss of nearly 76% of the originally mined data.

The `relevant.ids` file contains tweet IDs, user IDs, and the drug that was used to identify that tweet for relevance. The drugs are listed in the `drugs.txt` file.

The tweet content can be downloaded with the `download_tweets.py` file, released by Azadeh Nikfarjam (Arizona State University) as a compontent of her research group's 2015 work *Pharmacovigilance from social media: mining adverse drug reaction mentions using sequence labeling with word embedding cluster features*. The script requires BeautifulSoup.

## Drugs
The 334 drugs in the `drugs.txt` file represent the 81 drugs present in ADR tweets from the Nikfarjam 2015 study (available [here](http://diego.asu.edu/downloads/publications/ADRMine/drug_names.txt)), the New York State Department of Health [top 150 drugs](https://apps.health.ny.gov/pdpw/DrugInfo/DrugInfo.action) list, and Chemical and Engineering News' [2014 top 50 drugs list](http://cen.acs.org/content/dam/cen/supplements/CEN-supplement092014.pdf).

## Relevancy Screening
Tweets were mined using the Twitter API and screened automatically for relevancy. All tweets containing external URLs, any of a small set of terms related to salesmanship (e.g. *sale*, *promo*, *cheap*, *free shipping*), or lacking the searched-for drug name in the tweet text itself were discarded.

## Use
This corpus is freely available to the academic community. By downloading Twitter data, you agree to follow the current [Twitter terms of service](https://twitter.com/tos), which requires not to redistribute the tweet content and to delete tweets that are marked deleted in the future.

## Contact
Please email `ericbenz` at `brandeis` dot `edu` with questions or concerns.
