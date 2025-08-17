# BlinkItScraper

BlinkItScraper is a web scraping project built using Python, Selenium, and Django.  
It allows users to input product details through a web interface, scrapes data from BlinkIt, and displays the results in a structured format.

---

## Features
- User-friendly interface with Django templates (`index.html`, `home.html`, `results.html`)
- Selenium-based automated scraping of BlinkIt
- Clean display of scraped data in the results page
- Error handling for failed scraping attempts

---

## Requirements
- Python 3.8 or higher
- Google Chrome (latest version recommended)
- ChromeDriver (matching your Chrome version)
- Git

---

## Installation and Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/<your-username>/BlinkItScraper.git
   cd BlinkItScraper
   ```
   
2. **Set up a virtual environment (recommended)**
   ```bash
   python -m venv venv
   source venv/bin/activate   # On macOS/Linux
   venv\Scripts\activate      # On Windows
   ```
   
3. **Install Dependencies**
   ```bash
   pip install selenium chromedriver pandas openpyxl requests django
   ```
   
4. **Set up Chromedriver**
   - Download ChromeDriver from: https://chromedriver.chromium.org/downloads
   - Ensure it matches your installed Chrome version.
   - Place it in your PATH or inside the project root folder.

5. **Run the Database Migrations and Start the Django server**
   ```bash
   python manage.py migrate
   python manage.py runserver
   ```

6. **Access the App**
   Your app will be running on ```http://127.0.0.1:8000/```.

---
# Usage

- Enter the product name on the home page.
- The scraper will search for the product on BlinkIt.
- Results will be displayed on the results page with product details.

---
# Troubleshooting

1. Permission denied (publickey) when pushing to GitHub
   Make sure your SSH key is added to GitHub

2. ChromeDriver errors
   Ensure your ChromeDriver version matches your installed Chrome browser.

3. Selenium errors
   Verify that the selectors used in the scraper match BlinkIt’s latest HTML structure.

---
# Contributing

Feel free to fork the repository and submit pull requests with improvements!
