# 📧 Email Scraper

A simple Python-based email scraper that crawls a target URL and extracts email addresses found in the pages it visits.  

## ✨ Features

- Starts from a given URL and follows links to discover new pages.
- Extracts email addresses from page content using regex.
- Keeps track of already-scraped URLs to avoid repeats.
- Stops after 100 pages (configurable in the code).

## 🛠️ Requirements

- Python 3.x  
- [requests](https://pypi.org/project/requests/)  
- [beautifulsoup4](https://pypi.org/project/beautifulsoup4/)  
- [lxml](https://pypi.org/project/lxml/)  

Install dependencies:

```bash
pip install requests beautifulsoup4 lxml
```

## 🚀 Usage (authorized environments only)

1. Clone this repository:

```bash
git clone https://github.com/RazPriel/Email-Scrapper.git
cd Email-Scrapper
```

2. Run the script:

```bash
python3 email_scraper.py
```

3. Enter the target URL when prompted:

```
[+] Enter target url to scan: https://example.com
```

4. The script will crawl up to 100 pages from the starting URL and print discovered email addresses:

```
[1] Processing https://example.com
[2] Processing https://example.com/about
info@example.com
support@example.com
```

Stop it safely with `Ctrl + C`.

## 📝 Notes

- The maximum pages (100) is hardcoded in the script; adjust `if count == 100:` if needed.
