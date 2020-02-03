# Market_Analytica
A Repository for Stock Market Analytics



# Repository Directory
Most of the files and folders are self explanatory. However, if you are looking for something swiftly, you can find it using the following.

1. Archive - Old files dedicated to analyzing "Fortune 100" stocks
2. Plots - All of the wonderful visuals that were made to summarize the analytics in the Repo
3. Resources - Storage for data used in the S&P500 analytics and data collection
4. Scripts - Code which was used to execute the data collection and analysis

# WHAT
This project houses data, scripts, and analytics for analyzing the Standard & Poor's Market Stock.


# WHY
First and foremost, this project was undertaken because of my curiosity and vested interest in understanding some of the outcomes of this project.

This analysis looks at answering several different and interesting questions one might have about the S&P500 over the past 2 decades.
-- Here are some of the questions that you might have that these analytics could help in deriving for you --

1. What kind of Sectors (industries) are present in current the S&P500 and are there some that clearly stand out as winners?
2. Are S&P500 stocks gaining value and are they returning increases in value that are beating the rest of the market?
3. How popular are these large Market Cap stocks and are they gaining interest from investors?
4. What are some of the best and worst performing stocks to invest in?
5. What are some of the best and worst performing sectors to invest in?
6. When there is economic downturn or rebound, what might be some good things to invest in?

-- Some Limitations -- 

Note there could be more depending on what you would like to determine with this analysis, but here are some common insights:

1. The list of companies used is the current S&P500 list. Note that the list is dynamic and companies move in and out all the time.
2. Data was limited to only the 375 stocks that existed for all 20 years called, so it does not include all 500.
3. While having a whopping 375 different stocks is great, more stocks should be considered before making significant investments as these only represent the largest of the large-cap companies.
4. Up-turn and down-turn periods are defined using peak-to-peak time frame of the S&P 375 index average.
5. The rebound period analyzed was from th bottom peak of the End Of Year 2018 dip to the end of data called (present) since there has not be a major flattening or downturn in the market to date.


# WHEN
The data collection and analysis for this project occured between December 2019 - January 2020.


# HOW (and notes)
1. Data was crunched by first defining a scope of project. (What is the story we want to tell?)
2. After finding an API the suited the needs of the project (Alpha Vantage), it was decided to pull the past 20 years of daily S&P500 stock data. 
	1. Financial Data is pretty difficult to come by, and even harder when you want it for free.
	2. The Script to query the API was written in a Jupyter Notebook, Stock_Query.ipynb. The notebook was written in Python using the Requests library and Pandas to pull and manage storage of data. 
	3. Several API Query Scripts were written in order to produce more efficient data collection (AV's Freemium limits call to 5/ machine time minute). The efficiency of our data queries was improved by 40%! Up from ~4.8 to 6.75 calls per minute by using different call techniques!
3. After data was collected and sequentually stored in a CSV file (~2.2M rows), data was called and munged via use of the Stock_Analytica.ipynb. At this point, the data was cleaned by only considering stocks with the full 20 years of data, leaving 375 contenders (now the S&P375).
4. Many aggregations were performed on this data, which can be viewed in the script. The aggregates are also apparent in the plots that were created using Pandas and Matplotlib.
5. Review and Celebration!


tldr: Define Project Scope -> Alpha Vantage API Queries -> Jupyter Notebook .ipynb for data cleanup, aggregations, and visualizations


# WHO (and my role)
Good question. This project was initally undertaken by myself and a group of 3 associates to analyze an aggregate of the Fortune 500 List. During this project, I was responsible for delivering all of the stock data via use of an API request script.
This initial project yielded a mix of unsatistying results (mainly driven by skewed data - Fixed by including more!), and I was interested in the followup analysis.
I created the analysis portion of this, S&P500, project.


tldr: The project started out as a seperate group project looking at the Fortune 500. I was interested in more so I continued on, and I created all of the content associated with this specific repository.


# Future
I am interested in developing some of the skills I learned here into creating a day-trading app! (Automated ROI Value)
I am also interested in running a good portion of this data through Scikit-Learn for modeling purposes, most probably incorporated into the day-trading app.


tldr: Day-Trading app, Machine Learning on Stock Data


# Technical Stuff

Development Environment:
1. Jupyter Notebook
2. Visual Studio Code

Libraries:
1. Pandas
2. Matplotlib
3. Time
4. Requests
5. Unix Shell (Bash)

Technologies:
1. .gitignore (api keys)
2. .gitattribute (Git LFS)

Hosting:
1. GitHub

Resources:
1. Google
2. Alpha Vantage
3. A good bit of Docs & Stack Overflow
4. Friendly Associates