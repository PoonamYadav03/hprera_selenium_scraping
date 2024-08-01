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
