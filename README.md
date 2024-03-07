Riley Taylor

UTA Data Analytics Bootcamp

Module 11 - Data Collection (BeautifulSoup and Web Scraping)




## Description

This contains my submission for module 11 of the UTA Data Analytics Bootcamp. We were tasked with completing two supplied jupyter notebooks that would test the use of the BeautifulSoup library and our understanding of the data.


## Requirements

To be able to run the jupyter notebooks, you will need the following libraries:

-   splinter
-   BeautifulSoup
-   pprint (exclusive to part_1)
-   matplotlib (exclusive to part_2)
-   pandas (exclusive to part_2)

Also make sure that you have a compatible chrome-driver available to run the `browser=Browser('chrome')` code. Alternatively, you can try using the requests library and feeding the result of `requests.get(url).text` to BeautifulSoup, but there is a shortfall to that because some scripted websites will generate html in a browser that the requests library will not find. 

The project was run using Python 3.10.13. 

## Installation

Install by cloning the repo and using the tool of your choice to handle the jupyter notebooks. 

## Repo Overview 

`/Resources/` contains the csv file `mars_data.csv` that we generated in `part_2_mars_weather.ipynb`

`part_1_mars_weather.ipynb` is the jupyter notebook that focused on grabbing and reading text from specific tags [here](https://static.bc-edx.com/data/web/mars_news/index.html)

`part_2_mars_weather.ipynb` is the jupyter notebook that focused on grabbing and reading mars weather data from the table [here](https://static.bc-edx.com/data/web/mars_facts/temperature.html), and then visualizing/analyzing some questions about that data. 



## Notes

The `mars_data.csv` contains a column called `time_elapsed` which measures the time difference from the date of that entry to the first entry in the data set. We used this to create the weather plot that helped visualize the length of a mars year. It is measured in days.  



-----------------------------

## Sources 
### Note - many of these were used for knowledge acquisition, with no direct reference to their content in this assignment. 


Mars Temperature Data
https://static.bc-edx.com/data/web/mars_facts/temperature.html

python - How do I get the row count of a Pandas DataFrame? - Stack Overflow
https://stackoverflow.com/questions/15943769/how-do-i-get-the-row-count-of-a-pandas-dataframe

pandas.core.groupby.GroupBy.mean — pandas 0.25.0 documentation
https://pandas.pydata.org/pandas-docs/version/0.25.0/reference/api/pandas.core.groupby.GroupBy.mean.html

python - Bar graph from dataframe groupby - Stack Overflow
https://stackoverflow.com/questions/40313727/bar-graph-from-dataframe-groupby

python - Keep only date part when using pandas.to_datetime - Stack Overflow
https://stackoverflow.com/questions/16176996/keep-only-date-part-when-using-pandas-to-datetime

pandas.DataFrame.to_csv — pandas 2.2.1 documentation
https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.to_csv.html


In addition, ChatGPT was consulted for assistance with converting the time deltas in the column `time_elapsed` to just days, to clean up the final visual in the second python notebook. 