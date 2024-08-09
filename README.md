# Key Events of the 20th Century - Web Scraping Project

This project involves web scraping key events of the 20th century from a Wikipedia page and analyzing the frequency with which various countries are mentioned in these events. The analysis includes generating a plot that visualizes how many times each country is mentioned, specifically focusing on countries that are mentioned more than once.

## Project Overview

The project involves:
1. **Web Scraping**: Extracting key events of the 20th century from the relevant Wikipedia page.
2. **Data Preparation**: Cleaning the extracted text data by removing unwanted characters (like apostrophes) and ensuring consistent formatting.
3. **Counting Mentions**: Counting the occurrences of each country name in the text data.
4. **Visualization**: Creating a bar plot that shows the frequency of countries mentioned more than once, using a dark blue color for the bars.

## Web Scraping Details

The web scraping process focuses on extracting events listed under the 20th century section of the Wikipedia page. The script identifies and extracts relevant sections of the page, then processes the text to isolate mentions of different countries.

### Libraries Used

The following Python libraries are used in the web scraping and analysis process:

- `requests`: To fetch the webpage content.
- `BeautifulSoup` (from `bs4`): To parse and extract information from the HTML content.
- `pandas`: For data manipulation and analysis.
- `matplotlib`: For generating the plot.
- `seaborn`: For enhancing the aesthetics of the plot.



### Findings

- **France** is the most frequently mentioned country, followed by **Germany** and **Italy**.
- The plot suggests a focus on European countries within the context of the key events of the 20th century.
- The skewness in the data indicates that a few countries are mentioned frequently, while many others are mentioned only once or not at all.

### Prerequisites

Ensure that you have the following Python libraries installed:

- `requests`
- `beautifulsoup4`
- `pandas`
- `matplotlib`
- `seaborn`

You can install these packages using pip:

```bash
pip install requests beautifulsoup4 pandas matplotlib seaborn
