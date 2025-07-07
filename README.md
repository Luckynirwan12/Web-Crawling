# Web Crawling
## 📧 Email Crawler & Extractor 🔍
This Python program crawls a website using its sitemap.xml and extracts all the email addresses found across the listed pages. The emails are saved into a clean CSV file.

## 📥 Input
- A valid URL to a website's sitemap.xml.
Example:

      https://yourdomain.com/sitemap.xml

## 📤 Output
- A CSV file named Emails.csv containing all the extracted email addresses:

      Email
      example1@domain.com
      example2@domain.com
      ...

## ⚙️ Features
- Crawls thousands of web pages listed in a sitemap.

- Extracts unique email addresses using regular expressions.

- Bypasses SSL certificate errors when needed.

- Saves results in a structured CSV file using pandas.

- Displays progress with a progress bar using tqdm.

## 🛠️ Technologies Used
- requests, requests-html – for HTTP requests

- BeautifulSoup – to parse sitemap XML

- re – to extract email patterns

- pandas – to store and export results

- tqdm – for progress tracking

## 🚀 How to Run
1. Install required packages:

       pip install requests requests-html pandas beautifulsoup4 tqdm
2. Run the script and update the sitemap URL as needed:

       links_data_arr = get_urls_of_xml("https://thapar.edu/sitemap.xml")
3. Output: A CSV file named Emails.csv will be created with all found email addresses.
