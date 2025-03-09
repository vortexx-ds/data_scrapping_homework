# Indian Military Aircraft Data Scraper

## Project Description
This project is focused on practicing web scraping and data analysis using Python. The script extracts data from the Wikipedia page titled "[List of active Indian military aircraft](https://en.wikipedia.org/wiki/List_of_active_Indian_military_aircraft)", specifically the table containing the list of active military aircraft. The extracted data is saved into a CSV file for further analysis.

---

## How the Script Works
1. **Fetch the Web Page:**
   - The script uses the `requests` library to send a GET request to the Wikipedia page.
   - A `User-Agent` header is added to ensure successful connection with the website.

2. **Parse the Web Page:**
   - The `BeautifulSoup` library is used to parse the HTML content of the page.
   - It identifies the `<table>` tag with the class `wikitable` that contains the desired data.

3. **Extract Data:**
   - The script iterates through the rows of the table (`<tr>` tags), skipping the header row.
   - For each row, it extracts key information like:
     - Aircraft Type
     - Role
     - Country of Origin
     - Quantity

4. **Save Data:**
   - The extracted data is stored in a structured format using the `pandas` library.
   - The data is saved into a CSV file (`indian_military_aircraft.csv`) for further analysis.

---

## Steps to Run the Script
Follow these steps to run the script on your system:

1. **Install Required Libraries:**
   Ensure that the necessary Python libraries are installed. Use the following command:
   ```bash
   pip install requests beautifulsoup4 pandas
