﻿# webscraping-

this is just a simple web scrapping  script to scrape covid-19 data from mohfw website. This scipt is developed using the help https://www.codementor.io/@oluwagbengajoloko/how-to-scrape-data-from-a-website-using-python-n3fmtc63q

=======================================================================
Lines one - three Imports all the packages required to run the appliance.

Line six we have a tendency to outline the fuction scrape_data that takes a address parameter.

Line eight we have a tendency to create a get request to the address victimization the get methodology of the requests library.

When creating HTTP requests with the request library, it's vital to line a timeout inclose the server doesn't respond in a very timely manner. This prevents your program from hanging indefinitely whereas awaiting a response from the server.

Line nine we have a tendency to produce a beatuful soup tree structure from the content of the response from the server. This object is straightforward to navigate and search through.

Line eleven we have a tendency to search throught the beatufiful object soup to search out the second table within the document that contains the information we wish victimization the it's find_all methodology. The beautifulsoup object's find_all methodology searches for all HTML tags that match the filter/search-term within the tree structure.


Line thirteen This line of code selects all the tr components wherever
the parent could be a tbody component from the table. tr components represents the table rows.

Line fifteen the primary row ussually contains the header cells. we have a tendency to serch throught the primary row within the rows list to urge the text values of all th components in this row.
we additionally guarantee to get rid of the all trailing whitespaces within the text victimization the rstrip python string methodology.

Line seventeen - twenty two This opens a file and creates a brand new file object. The w mode is employed to make sure the file is open for writing.
First we have a tendency to write the header row, then loop through the remainder of the rows ignoring the primary row to urge the information contained at intervals and write the information for all those rows to the file object.

Line twenty five -27 we have a tendency to check to make sure the module is run because the main program and decision the perform scrape_data with a specific address to scrape the information.


# on a the terminal run the command below to scrape the data

# Run the commands below to install the beatifulsoup and requests library

# pip install requests
 
# pip install beautifulsoup4

# python automaticscipt.py

