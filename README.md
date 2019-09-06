# HistDataScraper
A simple web scraper that downloads forex calendar data from ForexFactory.

The download is managed in packets of weeks, stating on a sunday.\
The chosen timezone is Eastern Standard Time (EST) time-zone WITHOUT Day Light Savings adjustments, to mach the data from https://www.histdata.com\.\
The program starts at the first possible download date, jan 7 2007, and ends with the last completed week.\
Any later executions of the program checks for the date of the last entries and updates the list incremental.\
The out put file will be located in the working directory and be called forex_factory_catalog.csv

It is required to have firefox installed and a version of geckodriver in the same folder as the program. (https://github.com/mozilla/geckodriver/releases\).\
All other requirements are within requirements.txt.\
You can easily install them with 'pip install -r requirements.txt'.
