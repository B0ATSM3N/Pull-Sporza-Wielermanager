Wielermanager Startlist Checker
===============================

The Wielermanager Startlist Checker is a Python script that checks if riders listed in an Excel sheet are participating in races of a specified year according to the startlists available on the website `www.procyclingstats.com`. The script retrieves the race names and numbers from an Excel sheet, builds the startlist URL for each race and extracts the startlist table for that race from the HTML content of the URL. It then loops through the rider names listed in another Excel sheet, cleans them and checks if they are present in the startlist table for each race. The script writes the rider names, the number of races they are participating in and the results (0 or 1) for each race to a new sheet in the same workbook. The script also updates the number of races each rider is participating in on the original rider sheet.

Requirements
------------

-   Python 3.x
-   requests module
-   BeautifulSoup module
-   openpyxl module

Installation
------------

1.  Clone this repository or download the zip file and extract it.

2.  Install the required modules using pip:

    Copy code

    `pip install requests
    pip install beautifulsoup4
    pip install openpyxl`

Usage
-----

1.  Prepare two Excel sheets named `races` and `riders` in a file called "riders.xlsx". The `races` sheet must contain the columns `Race name` and `Race number`. The `riders` sheet must contain the columns `Team`, `Rider name` and `Value`. The first row of each sheet should be the column header. You can copy the data from the "Rennerslijst" provided on the wielermanager website.
2.  Add the race names and numbers to the `races` sheet.
3.  Add the rider names, teams and values to the `riders` sheet.
4.  Run the script in a terminal or in an IDE.
5.  The script will create a new sheet named `results` in the same workbook with the results of the startlist check.

Disclaimer
----------

The script may not work if the structure of the `www.procyclingstats.com` website changes. The script was last tested on 2023-03-20.
