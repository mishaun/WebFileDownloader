# WebFileDownloader

This repo will contain a jupyter notebook file that will perform the following tasks:

1.  Open chrome webdriver and navigate to EnergyNet - a oil and gas auction/asset page
2.  After logged in, it will load the account's previous won lots or assets
3.  Based on an exported spreadsheet, all the lots won in this account will be stored
3.  The script will then access this spreadsheet (through pandas), and it will create a directories based on the won lot names.
    These created directories serve as destination folders for lot's data package files
4.  The script with then query each lot number with automation web commands and navigate to the lot's listing page
5.  It will attempt to download the consolidated package hosted on webpage, if not found, it will navigate back to the listing page.
6.  The script will then enter the older style data room, where each document is available one by one.  The script will then click
    each link and download the files.
7.  Finally, the script will move pdf's from the downloads directory into the destination folder for the lot    
