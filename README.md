Creating a corpus for a BS program's courses involves several steps, including web scraping, data cleaning, and organizing the data into different files based on specific criteria. Here's an outline of the process:

Web Scraping: Utilize tools like BeautifulSoup or Wikipedia API to scrape information about courses offered in the BS program from relevant sources such as university websites or online course platforms.

Data Cleaning: Remove any unnecessary spaces, special characters, and broken links from the scraped content using regular expressions or other text processing techniques.

Organization: Organize the cleaned data into different files based on the provided specifications:

a. corpus.csv: This file will contain columns for topic, content, URL, type, vocabulary size, and word count.

b. tokens.csv: Include columns for topic, stems, and lemmas.

c. vocabulary.csv: Include columns for topic and unique words.

d. readability.csv: Compute readability scores for each topic using tools like textstat, specifically Flesch-Kincaid grade level.

e. pos.csv: Generate a file with columns for topic and data with POS tags.

Classification Model: Train a logistic regression model using the readability scores as the target variable (y) and other features as predictors.
