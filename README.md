# Anewstip-Journalist-Scraper
This project is a GUI-based web scraper for extracting journalist information from Anewstip based on a list of keywords. It uses Selenium, BeautifulSoup, and Tkinter to automate the browser, scrape profiles, and save data to an Excel file.  Features Keyword-based Search: Load keywords from a .txt file (one keyword per line). 


This project is a GUI-based web scraper for extracting journalist information from Anewstip based on a list of keywords.
It uses Selenium, BeautifulSoup, and Tkinter to automate the browser, scrape profiles, and save data to an Excel file.

Features
Keyword-based Search: Load keywords from a .txt file (one keyword per line).

Automated Browser Launch: Opens Chrome, where you manually log into Anewstip.

Scraping Journalist Profiles: Extracts:

Journalist Name

Title

Outlet

Email (if available)

Topics

Live Excel Updates: Saves results to .xlsx while scraping.

Multi-page Support: Automatically navigates through multiple result pages for each keyword.

GUI Interface: No need for command-line usage, thanks to Tkinter.

Requirements
Install the dependencies using:

bash
Copy
Edit
pip install -r requirements.txt
requirements.txt

nginx
Copy
Edit
selenium
beautifulsoup4
pandas
openpyxl
Additional Requirements:

Google Chrome installed.

ChromeDriver (make sure chromedriver matches your Chrome version and is in your system PATH).

How to Use
Clone this repository:

bash
Copy
Edit
git clone https://github.com/yourusername/anewstip-scraper.git
cd anewstip-scraper
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Run the app:

bash
Copy
Edit
python app.py
In the GUI:

Click “Load Keywords File” and select a .txt file with your keywords.

Click “Choose Save Location” to select where to save results (.xlsx).

Click “Launch Anewstip”, then log in manually when Chrome opens.

Click “Start Extract” to start scraping.

Example Keyword File
nginx
Copy
Edit
sports
politics
technology
Output Example
The resulting Excel file will look like:

Keyword	Name	Title	Outlet	Email	Topics
sports	John Doe	Reporter	ESPN	john@espn.com	Football, Basketball
politics	Jane Smith	Journalist	NY Times	jane@nytimes.com	Elections, Policies

Code Overview
app.py
Contains:

GUI setup with Tkinter

Selenium logic for navigating Anewstip

BeautifulSoup parsing of journalist data

Live Excel file creation with openpyxl

Possible Improvements
Headless browser support.

Proxy & captcha handling.

Export in multiple formats (CSV, JSON).

Error logging.

