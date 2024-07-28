# Manga Scraper

This Python script allows you to download and convert manga chapters into PDF format from a specified manga website. It retrieves images from the specified chapter, downloads them using multithreading, converts the images to PDF, and merges them into a single PDF file per chapter. The script includes error handling and logging for reliable operation and easier debugging.

## Features

- Scrapes image URLs from manga chapters.
- Downloads images using multithreading for faster performance.
- Converts downloaded images to PDF format.
- Merges individual PDFs into a single PDF file for each chapter.
- Automatically handles file cleanup and directory management.

## Requirements

- Python 3.10+
- BeautifulSoup4
- Requests
- Pillow
- fpdf
- PyPDF2

## Installation

1. Clone the repository:

   git clone https://github.com//manga-scraper.git
   cd manga-scraper

2. Install the required dependencies:

   pip install -r requirements.txt

## Usage

1. Run the script:

   python manga_scraper.py

2. Enter the URL of the manga when prompted.

3. Select which chapters to download by typing 'Y' for Yes, 'N' for No, or 'C' to Cancel.

## Logging 

The script includes detailed logging to help you monitor the download and conversion process and diagnose any issues. Logs are printed to the console with timestamps and log levels.

1. Example:-

	Enter the URL of Manga: https://example.com/manga/series-name
	URL: https://example.com/manga/series-name
	Chapters: {'Chapter 1': 'https://example.com/manga/series-name/chapter-1', 'Chapter 2': 'https://example.com/manga/series-name/chapter-2'}
	Chapter 1: https://example.com/manga/series-name/chapter-1
	Y for Yes, N for No, C for Cancel
	Download? (Y/N/C) Y
	Downloading Chapter 1 From https://example.com/manga/series-name/chapter-1
	Downloading 20 pages
	Downloaded Chapter 1 successfully
	Chapter 2: https://example.com/manga/series-name/chapter-2
	Y for Yes, N for No, C for Cancel
	Download? (Y/N/C) N

## Contributing

Contributions are welcome! Please fork this repository and submit a pull request for any improvements or bug fixes.