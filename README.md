# University Website Data Analysis and Visualization Tool

The University Website Data Analysis and Visualization Tool is a web scraping application designed to extract data from three different university websites in Pakistan. By scraping five web pages from each university, the tool collects valuable information for analysis and visualization.

## Features

- **Web Scraping:** Utilizes Python's `requests` and `urllib` libraries to fetch webpage content.
- **Natural Language Processing (NLP):** Employs the `spacy` library for tasks such as noun and verb extraction.
- **Comprehensive Analysis:** Compares university websites in terms of adjectives, verbs, and nouns, providing insights into their content emphasis.
- **Graph Visualization:** Constructs a graph representation using `networkx` and `matplotlib`, highlighting relationships between nouns.
- **Key Metrics:** Provides metrics such as the number of connected components and the top 10 nouns with the highest degree.
- **Proximity Analysis:** Allows users to explore noun proximity to the term "quality" within a specified distance.

## Installation

Install the required libraries:

```bash
pip install networkx spacy pandas matplotlib requests urllib3 beautifulsoup4 dframcy
python -m spacy download en_core_web_sm
```

## Usage

1. **Prepare URLs:** Modify the `urluaar1`, `urluet`, `urlcomsats1`, and `urlcomsats2` variables with the desired URLs of the university websites you want to scrape.
   
2. **Run the Code:** Execute the code to scrape the specified university websites and store the data in separate text files: `Uaar.txt`, `Uet.txt`, and `Comsats.txt`.
   
3. **Choose University:** Enter a number (1, 2, or 3) to choose a university website for analysis.
   
4. **Analysis:** The tool performs analysis on the chosen university's web content, including extracting nouns, adjectives, and verbs, displaying their frequencies, constructing a graph showing noun connections, and displaying top 10 nouns with the highest weighted degree. Additionally, it prints the five words near the word "Quality" within the selected university's content.

Note: Ensure you have a stable internet connection to fetch the website data successfully. Remember to have the required permissions to scrape the university websites, as some websites may have restrictions or terms of use.
