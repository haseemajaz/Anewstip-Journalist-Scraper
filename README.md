# Anewstip Journalist Scraper

A Python-based GUI tool that scrapes journalist information from **Anewstip** based on a list of keywords. It uses **Selenium**, **BeautifulSoup**, and **Tkinter** to provide an easy-to-use interface for loading keywords, launching the browser, and saving the extracted data into an Excel file.

---

## Features

- **Keyword-based search:** Reads keywords from a `.txt` file (one keyword per line).
- **Automated scraping:** Extracts journalist profiles including:
  - Name
  - Title
  - Outlet
  - Email
  - Phone
  - Topics
- **Live Excel updates:** Data is saved in real time to an `.xlsx` file while scraping.
- **Duplicate avoidance:** Skips already saved records.
- **Multi-page scraping:** Automatically navigates through all result pages for each keyword.
- **GUI Interface:** No need to use the command line.

---

## Tech Stack

- **Language:** Python 3.x
- **Libraries:**
  - `selenium` – For browser automation.
  - `beautifulsoup4` – For parsing HTML.
  - `pandas` – For handling data and exporting to Excel.
  - `openpyxl` – For working with Excel files.
  - `tkinter` – For GUI interface.
  - `threading` – For non-blocking scraping.

---

## Installation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/Anewstip-Journalist-Scraper.git
   cd Anewstip-Journalist-Scraper
   ```

2. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Download ChromeDriver:**
   - Make sure you have Google Chrome installed.
   - Download the correct ChromeDriver from: https://chromedriver.chromium.org/downloads
   - Place it in your system PATH or the project directory.

---

## Usage

1. **Prepare Keywords:**
   - Create a `keywords.txt` file with one keyword per line (e.g., `technology`, `health`, etc.).

2. **Run the Script:**
   ```bash
   python Anewstip-Journalist-Scraper.py
   ```

3. **Steps in GUI:**
   - **Load Keywords:** Select your `keywords.txt`.
   - **Choose Save Location:** Pick where the Excel file will be saved.
   - **Launch Anewstip:** Opens Chrome browser. **Login manually**.
   - **Start Extract:** Automatically scrapes all journalist profiles and updates the Excel file live.

---

## Output

- The output will be an Excel file (`.xlsx`) with columns:
  ```
  Keyword | Name | Title | Outlet | Email | Phone | Topics
  ```

---

## Screenshot

*(Add a screenshot of the GUI and sample Excel output here.)*

---

## Notes

- You must log in to **Anewstip** manually before starting the scraping process.
- Chrome must stay open during the scraping.
- Avoid running too many keywords at once to prevent being blocked.

---

## License

This project is licensed under the MIT License.
