# RERA Data Scraper

## Overview

This project provides a Python script for scraping RERA (Real Estate Regulatory Authority) data from the HPRERA (Haryana RERA) website. It uses Selenium WebDriver to navigate through the listings, extract relevant information, and save it to an Excel file.

## Features

- **Load the RERA public dashboard page**: Opens the specified URL using Selenium WebDriver.
- **Click on listings**: Navigates through the listings and clicks on each to view detailed data.
- **Extract data**: Collects information including RERA Number, Name, GST Number, PAN Number, and Permanent Address from each listing.
- **Navigate back**: Returns to the main page to continue processing other listings.
- **Save to Excel**: Writes the collected data into an Excel file for easy access and analysis.

## Installation and Setup

### Clone the Repository
Clone the project repository from GitHub:

```bash
git clone https://github.com/PoonamYadav03/hprera_selenium_scraping.git
cd hprera_selenium_scraping
## Installation and Setup

### Create and Activate a Virtual Environment

1. **Create a virtual environment:**

    ```bash
    python -m venv env
    ```

2. **Activate the virtual environment:**

    - **On Windows:**

        ```bash
        .\env\Scripts\activate
        ```

    - **On macOS and Linux:**

        ```bash
        source env/bin/activate
        ```

### Install Dependencies

Install the required Python packages listed in `requirements.txt`:

```bash
pip install -r requirements.txt
## Code Details

The script `hprera_in.py` performs the following operations:

1. **Initialization**: 
   - Sets up ChromeDriver with necessary options and configurations.

2. **Loading Page**: 
   - Navigates to the specified URL.

3. **Clicking Listings**: 
   - Iterates through the listings, clicking each one to extract data.

4. **Extracting Data**: 
   - Retrieves information from each listing, including:
     - **RERA Number**: Extracted from the element containing 'Ref. No.'
     - **Name**: Extracted from the table cell labeled 'Name'
     - **GST Number**: Extracted from the table cell labeled 'GSTIN No.'
     - **PAN Number**: Extracted from the table cell labeled 'PAN No.'
     - **Permanent Address**: Extracted from the table cell labeled 'Permanent Address'

5. **Navigating Back**: 
   - Returns to the main page to process the next listing.

6. **Saving Data**: 
   - Writes the collected data to an Excel file named `scraped_data.xlsx`.







