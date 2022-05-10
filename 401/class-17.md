# Web Scraping
> Web scraping is a technique to automatically access and extract information from a website.

***Note: When web scraping, you must comply with the terms and conditions of each site, which may prohibit you from using the data for commercial purposes or block you.***

### Process overview

- Locate the data of interest.  There is a lot of code on a web page.  To locate the lines of interest, you must be familiar with HTML tags.

- Libraries like `requests` and `bs4` BeautifulSoup may help you parse the desired content.

- From the identified specific locations, download the data without spaming the site.

### Methods to prevent web scraping

Depending on the site, a number of methods could be inplace to prevent scraping:
- Blocking an IP address
- Blocking bot agents
- Blocking excess traffic
- Using CAPTCHA
- Obfuscating content with CSS
- Adding variable structure to pages
- Loading data straight into the DOM via AJAX -which leads to no visible data in the source document

---

### Resources

- [What is Web Scraping?](https://en.wikipedia.org/wiki/Web_scraping)
- [Web Scrape with Python in 4 minutes](https://towardsdatascience.com/how-to-web-scrape-with-python-in-4-minutes-bc49186a8460)
- [Track Amazon Prices](https://www.youtube.com/watch?v=Bg9r_yLk7VY)
- [Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/)

---

[Back to table of contents](../README.md)