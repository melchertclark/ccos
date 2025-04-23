URL Whiteboard Scraper
=====================

A simple utility to extract text content from multiple web pages listed in an Excel workbook.

Usage:
1. Double-click RUN_ME.bat (Windows) or RUN_ME.command (macOS)
2. Select your Excel workbook containing the "URL Whiteboard" sheet
3. Wait for the scraping to complete
4. The output files will be created in the same directory as your workbook

The Excel workbook should have a sheet named "URL Whiteboard" with:
- Column A: Labels for each URL
- Column B: The URLs to scrape

Output files:
- combined_YYYY-MM-DD_HHMM.txt: Contains the extracted text
- scrape_log_YYYY-MM-DD_HHMM.txt: Lists any URLs that failed to scrape 