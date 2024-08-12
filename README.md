# Key Events of the 20th Century - Web Scraping and Analysis Project

This project involves web scraping key events of the 20th century from a Wikipedia page and analyzing the frequency with which various countries are mentioned in these events. The analysis includes generating a plot that visualizes how many times each country is mentioned, specifically focusing on countries that are mentioned more than once. Additionally, the project involves network analysis of relationships between countries based on the events and extracting meaningful insights using various centrality measures.

## Project Overview

The project consists of the following steps:

1. **Web Scraping**: Extract key events of the 20th century from the relevant Wikipedia page.
2. **Data Preparation**: Clean the extracted text data by removing unwanted characters (like apostrophes) and ensuring consistent formatting.
3. **Counting Mentions**: Count the occurrences of each country name in the text data.
4. **Network Analysis**: Create a network graph that visualizes the relationships between countries based on the events, using centrality measures to identify key countries.
5. **Visualization**: Create a bar plot that shows the frequency of countries mentioned more than once, using a dark blue color for the bars, and visualize the network graph.

## Web Scraping Details

The web scraping process focuses on extracting events listed under the 20th-century section of the Wikipedia page. The script identifies and extracts relevant sections of the page, then processes the text to isolate mentions of different countries.

### Additional Considerations from the Chat

During the analysis, a specific focus was placed on ensuring the correct filtering of country names mentioned in the events:

- **Partial Matching of Country Names**: The project ensures that mentions of countries are detected even if the name is part of a longer string or phrase. For example, "Russia" will be correctly identified even if it appears as "Russian Federation" or in other similar forms.
- **Data Normalization**: Both the country names and the extracted text are normalized (converted to lowercase and stripped of extra spaces) to ensure consistent and accurate matching.
- **Debugging and Data Validation**: Debugging techniques were employed to ensure the correct identification and counting of country mentions, including checking the formatting and content of the extracted entities.

### Network Analysis

In addition to counting mentions, the project involves creating a network graph to explore relationships between countries based on the events. The network is analyzed using various centrality measures, including:

- **Degree Centrality**: Identifies countries that are directly connected to many other countries.
- **Betweenness Centrality**: Highlights countries that act as bridges within the network.
- **Closeness Centrality**: Determines countries that can spread information most efficiently through the network.

The network visualization is enhanced using tools like `NetworkX` and `pyvis`, which allow interactive exploration of the relationships.

### Libraries Used

The following Python libraries are used in the web scraping, analysis, and visualization process:

- `requests`: To fetch the webpage content.
- `BeautifulSoup` (from `bs4`): To parse and extract information from the HTML content.
- `pandas`: For data manipulation and analysis.
- `matplotlib`: For generating the plot.
- `seaborn`: For enhancing the aesthetics of the plot.
- `networkx`: For creating and analyzing network graphs.
- `pyvis`: For interactive network visualization.
- `spacy`: For natural language processing and entity recognition.

### Findings

- **France** is the most frequently mentioned country, followed by **Germany** and **Italy**.
- The network analysis identifies key countries that play central roles in the events of the 20th century.
- The plot and network graph suggest a focus on European countries within the context of the key events of the 20th century.
- The skewness in the data indicates that a few countries are mentioned frequently, while many others are mentioned only once or not at all.

## Prerequisites

Ensure that you have the following Python libraries installed:

- `requests`
- `beautifulsoup4`
- `pandas`
- `matplotlib`
- `seaborn`
- `networkx`
- `pyvis`
- `spacy`

You can install these packages using pip:

```bash
pip install requests beautifulsoup4 pandas matplotlib seaborn networkx pyvis spacy
