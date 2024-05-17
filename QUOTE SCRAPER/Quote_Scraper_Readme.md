## Quote Scraper and Quiz Game 📝💬
This Python script scrapes quotes from the website quotes.toscrape.com and presents a quiz game where the user has to guess the author of a randomly selected quote.

### Libraries Used
requests 🌐: For making HTTP requests.

BeautifulSoup 🍲: For parsing HTML documents.

csv 📋: For writing data to CSV files.

time ⏰: For adding delays between requests.

random 🎲: For random selection.

### Features
Scrapes quotes, authors, and author bio links from multiple pages.

Stores the scraped data in a list.

Presents a random quote to the user and asks them to guess the author.

Provides hints to the user if they guess incorrectly.

## How It Works
#### Scraping Quotes:

The script starts by initializing an empty list all_quotes to store the scraped data.

The base_url is set to "http://quotes.toscrape.com/", and the initial url is set to "/page/1".

The script enters a loop where it makes requests to the current page, parses the HTML, and extracts quotes, authors, and bio links.

If a "next" button is found, the script updates the url to the next page and continues scraping. The loop continues until there are no more pages.

#### Storing Quotes:

For each quote found on the page, the text, author, and bio link are extracted and appended to the all_quotes list.
Quiz Game:

A random quote is selected from the all_quotes list.

The user is presented with the quote and asked to guess the author.

The user has four guesses, and hints are provided if they guess incorrectly:

After the first incorrect guess, a hint with the author's birth date and place is given.

After the second incorrect guess, a hint with the author's first initial is given.

After the third incorrect guess, a hint with the author's last initial is given.

If the user runs out of guesses, the correct answer is revealed.

### Sample Output
![image](https://github.com/dharshii-22/DATA_SCIENCE_PROJECTS/assets/110839215/de1b38c0-3e38-4c0d-90f0-48c1c47235ce)
