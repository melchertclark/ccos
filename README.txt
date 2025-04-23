URL Whiteboard Scraper
=====================

A simple utility to extract text content from multiple web pages listed in an Excel workbook.

Setup Instructions:
1. Install Python 3.10 or higher from https://www.python.org/downloads/
2. Download this code (click the green "Code" button on GitHub and select "Download ZIP")
3. Extract the ZIP file
4. Open a terminal/command prompt and navigate to the extracted folder
5. Install required packages:
   ```
   pip install -r requirements.txt
   ```

Usage:
1. Run the script:
   ```
   python src/main.py
   ```
2. When prompted, select your Excel workbook containing the "URL Whiteboard" sheet
3. Wait for the scraping to complete
4. The output files will be created in the same directory as your workbook

Excel Workbook Format:
- Sheet must be named exactly "URL Whiteboard"
- Column A: Labels for each URL
- Column B: The URLs to scrape

Output Files:
- combined_YYYY-MM-DD_HHMM.txt: Contains the extracted text
- scrape_log_YYYY-MM-DD_HHMM.txt: Lists any URLs that failed to scrape

Optional Features:
- For faster processing, you can enable concurrent scraping:
  ```
  python src/main.py --concurrency 5
  ```
  This will process 5 URLs at a time (default is 1) 