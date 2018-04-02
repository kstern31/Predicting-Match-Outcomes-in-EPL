# Predicting-Match-Outcomes-in-EPL

1. Use the notebook in the data_collection_and_analysis/odds folder to scrape odds for previous seasons from oddsportal.com

2. Use the notebook in the data_collection_and_analysis/seasons folder to scrape team information for each match 
from whoscored.com for all seasons collected in step 1. This script takes a long time because it needs to load 
multiple pages per team, and is very prone to erroring out (due to elements not loading on the page), so the bulk of the
collection is within try/except blocks. You can consolidate parts of this notebook, as I had mistakenly not collected all the
data I wanted in one session.

3. EDA, data cleaning, and feature enguneering in the data_collection_and_analysis/composite folder

4. Modeling is done in the Data Transformation and Modeling notebook. pulled in 538 predictions from the spi_matches.csv.
