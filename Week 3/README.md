## Description
This folder includes materials covered during the 3rd week of the course (2 lectures of 2.5 hour duration). Regular expressions, native Python, as well as pandas imported read and write functions were introduced. Sublime text editor and Jupyter notebooks were used for executing the code. Topics covered include reading documents (csv, json, html, txt), writing files (csv, json), Regular expressions, parsing json as well as creating simple bot operating on Markvo chains. Packages covered include Pandas, JSON, RegEx, MarkovBot.

**Resources**
- [JSON formatter](https://chrome.google.com/webstore/detail/json-formatter/bcjindcccaagfpapjjmafapmmgkkhgoa?hl=en) - A google chrome extension which makes the JSON representation indented and highlighted (when viewed directly inside the browser).
- [Regex search](https://chrome.google.com/webstore/detail/regex-search/bcdabfmndggphffkchfdcekcokmbnkjl) - Another chrome extension which provides the opportunity of running a search on the webpage using regular extensions directly inside the borwser.
- [Online regex tester](https://regex101.com/) - an online tool for testing a regular expression on a sample text typed by the user. Also provides quick reference sheet and interactive explanation of the expression being tested.

**Homework**
```
1) Use read_html() function from the pandas library inside a for loop to get and print exchange rate data from
   rate.am for a week starting on June 1st and ending on 7th of June, 2017 included. The necessary steps to take
   are: 1) create the list of URLs to scrape, 2) create a for loop to iterate over the elements of that list and
   3) receive the data from each of them and 4) print it. (Hint: you may try for 2 URLs first, and then go for 7).
2) Use regular expressions to match (find) and print the value of S&P500 index from the Bloomberg website
   (website link: https://www.bloomberg.com/quote/SPX:IND, at the time of writing this the value of the index is
   2,434.51). Your regular expression must match any value of S&P500 even if it changes (e.g. whether it becomes
   1 or even 1,500,000.005, for example).
3) Create a for loop that will iterate over a given JSON file and print the keys followed by their values.
   The file (input string, which yet needs to be converted to JSON, as done in the classroom) and the expected
   output can be found in this Jupyter notebook: https://goo.gl/4IT7xG.
   NOTE: not more than one "if" and one "else" statements are allowed to use inside the for loop.
4) Download the AirPassengers.csv file from the Datasets folder in the Moodle, read that file to python and
   plot the "Passengers" column.
5) Use regular expressions to find the URL (the hyperlink) under the Next button on this webpage:
   http://quotes.toscrape.com/. 

Each point above is worth one mark. The overall homework is worth 5 marks (and 5% of the final grade).
You are encouraged to look trough the classroom materials, discuss with other students, yet your submission
should solely be your own work.

Anything additional is highly welcomed (yet, being highly welcomed does not generate additional points on homework).
```
