# READ 17

### Web Scraping

#### What is Web Scraping

- Web scraping, web harvesting, or web data extraction is data scraping used for extracting data from websites. Web scraping software may access the World Wide Web directly using the Hypertext Transfer Protocol, or through a web browser.

- While web scraping can be done manually by a software user, the term typically refers to automated processes implemented using a bot or web crawler. It is a form of copying, in which specific data is gathered and copied from the web, typically into a central local database or spreadsheet, for later retrieval or analysis.

### Important notes about web scraping

- Read through the website’s Terms and Conditions to understand how you can legally use the data. Most sites prohibit you from using the data for commercial purposes.

- Make sure you are not downloading data at too rapid a rate because this may break the website. You may potentially be blocked from the site as well.

### Scraping a Website

# Import libraries
import requests
import urllib.request
import time
from bs4 import BeautifulSoup

# Set the URL you want to webscrape from
url = 'http://web.mta.info/developers/turnstile.html'

# Connect to the URL
response = requests.get(url)

# Parse HTML and save to BeautifulSoup object¶
soup = BeautifulSoup(response.text, "html.parser")

# To download the whole data set, let's do a for loop through all a tags
line_count = 1 #variable to track what line you are on
for one_a_tag in soup.findAll('a'):  #'a' tags are for links
    if line_count >= 36: #code for text files starts at line 36
        link = one_a_tag['href']
        download_url = 'http://web.mta.info/developers/'+ link
        urllib.request.urlretrieve(download_url,'./'+link[link.find('/turnstile_')+1:]) 
        time.sleep(1) #pause the code for a sec
    #add 1 for next line
    line_count +=1