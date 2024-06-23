# Regex Operations, Web Scraping, and Text Processing

This script demonstrates several operations related to regex (regular expressions), web scraping, and text processing using Python libraries such as `nltk`, `re`, `requests`, `beautifulsoup4`, and `phonenumbers`.

## Tasks and Functionalities

### 1. Regular Expressions and Text Matching

The script includes a function `test_regex(regexp, text)` that tests various regular expressions on specified texts using `nltk.re_show`. It demonstrates matching patterns such as:
- Alphabetic characters `[a-zA-Z]+`
- Capitalized words `[A-Z][a-z]*`
- Patterns like `p[aeiou]{,2}t` for matching words like 'pat', 'pet', 'pit', 'pot', 'put'
- Numeric patterns `\d+(\.\d+)?` for matching numbers including decimals
- Complex patterns like `([^aeiou][aeiou][^aeiou])*` for specific sequences

### 2. Web Scraping

The script also includes functionality to fetch and extract information from a webpage using `requests` and `beautifulsoup4`:
- Function `fetch_url_contents(url)` retrieves the text content from a given URL using `requests` and parses it using `BeautifulSoup`.
- Function `extract_phone_numbers_and_emails(text)` extracts phone numbers and email addresses from the fetched webpage text using regex.

### 3. Text Normalization and Stemming

Demonstrates text normalization using NLTK's stemmers:
- Uses Porter and Lancaster stemmers (`PorterStemmer` and `LancasterStemmer`) to normalize tokens obtained from the webpage text.

### 4. Pattern Matching and Output

Uses regex to match specific patterns in a provided text and constructs outputs based on the matches:
- Matches patterns such as words starting with 'a', specific numeric formats, and structured text patterns.
- Constructs a message by combining extracted words based on regex matches.

## Outputs

- **Phone Numbers and Emails**: Extracted from a webpage using regex and web scraping techniques.
- **Stemmed Tokens**: Normalized tokens using NLTK stemmers (`PorterStemmer` and `LancasterStemmer`).
- **Pattern Matches**: Extracted words based on specified regex patterns from the provided text.

## Usage

To run the script:
1. Ensure all dependencies (`nltk`, `requests`, `beautifulsoup4`, `phonenumbers`) are installed.
2. Execute the script in a Python environment.
3. Review the console output for results of regex operations, web scraping, and text processing tasks.

## Dependencies

- `nltk`: For natural language processing tasks including tokenization and stemming.
- `requests`: For fetching data from URLs.
- `beautifulsoup4`: For parsing HTML content.
- `phonenumbers`: For parsing and formatting phone numbers.


