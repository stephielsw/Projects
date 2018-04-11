## Project Objectives
This project serves to allow user to keep a watchlist on the prices of kindle books which are of interest to the user.  Once the price of the books falls below $X amount (configured by user), user will receive an email alert on the drop of price.

## Components/tools
Scripts: 2 python scripts are created – watchlist.py to allow user to update watchlist and watchlistcheck.py which can be run daily to track kindle book prices.
Libraries: Requests, BeautifulSoup, Pandas, Re, OS, Subprocess, CSV, Time

## Description
Watchlist.py – once this script is run, user will be prompted to enter the title/author which he wants to search.  Upon data entry, the script will fetch the search results from Amazon and output to temp file tmpWatchlist.  TmpWatchlist file will be opened for user to update the books which he is interested to keep a watch on.  This list will then be output to Watchlist file.

WatchlistCheck.py – This script can be scheduled to run regularly.  Once run, it will based on the Watchlist file and go to Amazon to check the latest price.  The latest price will be updated to Watchlist and each row in Watchlist will be iterated to search for those rows where prices have dropped below $X.  User will receive an email alert with an attachment on this list of books.
