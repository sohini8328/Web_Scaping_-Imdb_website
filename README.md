# Web_Scaping_Imdb_website
Web scraping on IMDB webiste
Introduction
The purpose of this project is to conduct web scraping on the IMDB website and accumulate data of 100 movies across different genres and 100 actors who have worked in those chosen movies. The goal was to determine which genres were more profitable in particular decades. Additionally, the project explored the intricate relationship between the popularity and ratings of movies. It also examined the significance of experience or talent for winning awards in the Hollywood industry.

Tools and Technologies Used

Python: The primary programming language used for web scraping and data analysis.

BeautifulSoup: A Python library used to scrape and parse HTML data from the IMDB website.

Pandas: Utilized for data manipulation and analysis.

Matplotlib/Seaborn: Libraries used for data visualization.

Data Collection
To streamline the data extraction process, we focused on genre-organized webpages to gather all necessary movie information and actor-organized webpages for actor data. For the movies dataset, we selected 25 movies each from the genres: Comedy, Horror, Action, and Thriller, totaling 100 movies. Similarly, for the actors dataset, we selected 25 actors from each genre category, totaling 100 actors.

In total, 200 links (100 for movies and 100 for actors) were scraped using BeautifulSoup, and relevant features were extracted and organized.

Data Preparation
Movies Dataset:
Genres and actors were split into separate columns as they were originally concatenated.

The 'duration' column was dropped due to irrelevance.

Duplicates were identified and handled, replacing 'None' values with zeros.

Data types were adjusted, and extra characters were removed from 'gross_worldwide' and 'budget' columns.

A new column, 'return,' was created to calculate the ROI for each movie.

Actors Dataset:
No duplicates were found.

'None' values were replaced with zeros.

Data types for 'number_award_nominations' and 'number_award_wons' columns were corrected.

Movies Analysis:
ROI was calculated to identify the most profitable genres.

Pearson correlation analysis was conducted to explore relationships between movie attributes.

Actors Analysis:
The impact of award nominations and wins was assessed.

The relationship between experience (number of credits) and award success was examined.

Conclusion
The project demonstrated the power of web scraping to gather and analyze data from public websites like IMDB. Using BeautifulSoup, data from 100 movies and 100 actors were collected and analyzed to derive meaningful insights.

Key findings from the data analysis include:

Comedy was the most profitable genre: Comedy movies generated the highest returns on lower budgets compared to action movies, making them the most profitable genre in our dataset.

Decline in ROI over decades: The return on investment has decreased over time, possibly due to the rise of the TV industry and streaming services impacting traditional movie revenues.

Ratings and Popularity: The Pearson correlation revealed that higher IMDB ratings do not necessarily equate to greater popularity. High ratings may result from factors like storytelling quality, critical acclaim, or cultural impact rather than broad audience appeal.

Award Nominations as Predictors: Award nominations were found to be the strongest predictors of award wins. However, having more experience in various movie industry roles did not necessarily lead to more awards. This suggests that industry recognition through nominations is more crucial for winning awards than the number of credits.

While both datasets provided valuable insights, the analysis is limited due to the small sample size, selection bias, lack of full genre representation, and limited actor career data. Future studies could benefit from larger datasets and more diverse genre inclusion for more comprehensive conclusions. Use BLANK_README.md to get started Build With: This is the list of the libraries used by me to run this project were pandas,numpy, matplotlib.pyplot, matplotlib.ticker, re, os seaborn, beautiful soup and requests.

Getting Started: This is an example of how you may give instructions on setting up your project locally. To get a local copy up and running follow these simple steps. Prequisites: This is an example of software and how to install them. VS Code How to Run Clone this repository: https://github.com/sohini8328/Web_Scaping_-Imdb_website.git
