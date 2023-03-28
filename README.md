Procyclingstats.com Startlist Builder
=====================================

This script builds a startlist for selected races on procyclingstats.com, based on a list of rider names, teams and values in an Excel file.

The startlist is written to a new sheet in the same Excel file, with each rider's participation in each race indicated by a 1 or 0. The total number of races each rider is participating in is also calculated and added to the original rider sheet.

**Sporza Wielermanager**

This was created to return a list based on the riders provided by the game sporza wielermanager. You can download the 'Rennerslijst' and rename it to riders.xlsx.

**How to use**

1.  Ensure that the following modules are installed:

-   requests
-   bs4 (BeautifulSoup)
-   openpyxl

1.  Clone the repository or download the script and open it in your preferred Python IDE.
2.  Edit the **race_names** list to include the names of the races you want to build a startlist for. The script is currently set up for the 2023 season, but this can be changed by editing the **year** variable.
3.  Ensure that your rider data is stored in an Excel file with the following columns:

-   Column A: Rider team
-   Column B: Rider name
-   Column C: Rider value

1.  Update the **wb** variable to point to your Excel file.
2.  Run the script.
3.  The startlist will be written to a new sheet called "Startlist" in the same Excel file. The number of races each rider is participating in will be added to the original rider sheet.

**Limitations**

-   The script relies on the HTML structure of procyclingstats.com and may break if the site's structure changes.
-   The script currently only works for races on procyclingstats.com.
-   The script assumes that rider names, teams and values are stored in an Excel file with the specified column structure.

**Contact**

If you have any questions or feedback, please feel free to contact me via my Github profile.
