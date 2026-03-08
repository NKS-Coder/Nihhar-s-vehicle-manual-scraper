# Nihhar-s-vehicle-manual-scraper
n8n workflow for scraping vehicle manual PDFs and uploading them to cloud storage.

# Car Vehicle Manual Scraper

Automation pipeline for discovering, validating, and collecting vehicle manual PDFs from indexed web sources.

## Project Overview

This project uses **n8n automation workflows** to scrape vehicle manual PDFs across multiple manufacturers and year ranges, validate extracted files, and upload them to cloud storage automatically.

The workflow is designed to automate manual document collection and reduce repetitive data gathering.

---

## Key Features

• Automated vehicle manual scraping  
• Supports multiple manufacturers and year ranges  
• Regex-based PDF extraction from HTML pages  
• Batch processing with delays to prevent server overload  
• Validation of manual year ranges (2000–2026)  
• Automatic cloud upload using Google Drive integration  

---

## Workflow Architecture

The automation pipeline follows these steps:

1. Generate manufacturer and year catalog URLs  
2. Fetch index pages from the manual database  
3. Extract detail page links using regex filters  
4. Parse detail pages to locate PDF manual files  
5. Validate manual metadata and year range  
6. Download PDF documents with retry handling  
7. Upload verified files to cloud storage  

---

## Tech Stack

- n8n Workflow Automation
- JavaScript Function Nodes
- HTTP Request Nodes
- Regex Parsing
- Google Drive API
- Cloud Storage Integration

---

## Setup Instructions

1. Import the JSON workflow into **n8n**
2. Reconnect your **Google Drive credentials**
3. Replace the target folder ID
4. Run the workflow using the **Manual Trigger**

---

## Future Improvements

- Support additional vehicle manufacturers
- Add duplicate file detection
- Store metadata in a database
- Schedule automated runs with cron triggers
- Implement monitoring and logging

---

## Author

Nihhar K. Sonee

---

© 2026 Nihhar K. Sonee  
This repository is shared for portfolio and demonstration purposes only.
Unauthorized academic submission or plagiarism of this work is prohibited.
