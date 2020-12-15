# Web_Scraping_Indeed

The following project works with beautiful soup to scrape indeed.com to provide information about the salaries of various data science jobs across the world. This project aims to answer the question of whether or not data science as a field of work in the year 2020 is compensated equally across the planet as one would expect that such a lucrative industry would provide the same salary to individuals across the planet as the labour is highly skilled labour. In order to answer this question there was a need to determine the salary of data science postings across multiple locations, convert these salaries into a similar currency based on local purchasing power and then create a set of models to determine whether or not the adjusted salaries are tied to location. 

The general form of this project follows the following pseudo-code:
- Scrape the web for the data that is desired
- Append the values to a dataframe 
- Clean the dataframe using regex and pandas
- Utilise the concept of Purchasing Price Parity(PPP) to create a standardized salary across the board
- Run multiple models on the dataframe with PPP included
- Fit the best model and answer the general question posited at the start of the project.

The packages that were used throughout this project were as follows
* BeautifulSoup
* Selenium
* Pandas
* Scikit-learn
* NumPy
* Seaborn

Based on the results, it seems as though a simmilar standard of living is provided to Data Scientists across the world within their home country. However when it comes to international standards, the salaries are not comparable with western salaries being much higher than their counterparts elsewhere. With this in mind, the salary that is provided to an Indian Data Scientist in India is similar to that of an American or Canadian Data Scientist in the United States or Canada. This is interesting as it can serve as an indicator that the desire for this work across the world is about the same. This calculation does hinge upon the belief that the PPP that was provided by OECD is indeed an accurate way of assessing the value of the pound, dollar, and rupee against each other.  


NB: This web scraper was created in the summer of 2020, and it was quite common to have the salary posted alongside the job posting at this time. However currently, it is far more difficult to pull a salary with a web scrape as the salaries are not listed as frequently as they used to be listed on indeed.com. 


