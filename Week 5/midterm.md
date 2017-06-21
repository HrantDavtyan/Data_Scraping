<h2 align="center">Midterm Exam</h2>

<p align="center">19 June 2017</p>

<p align="center">Exam Duration: 1 hour 15 minutes</p>

<h2 align="center">Part 1 – Multiple-choice questions (10 points)</h2>

**Question 1**

The following code is used for reading a local file from the current directory. Find the mistake.
```
import json

with open("some_file.json","r") as f:
	my_file = json.dumps(f)
```
1. some_file.json was opened but not closed, which is compulsory thing to do,
2. the dumps()is used for writing files and cannot be applied to read-only files,
3. f is a file name, which means it should be provided inside quotes as "f",
4. single equal sign is used for assign and not for comparison purposes, which means the last line should be changed to my\_file == json.dumps(f).

**Question 2**

Which of the following statements is wrong?

1. read_html() function from the Pandas library can be used for reading tables in HTML.
2. findall() function from the re (regular expressions) library returns a list of matching strings.
3. If an expression to be matched includes at least one digit, then both "\d*" and "\d+" regular expressions will match the expression.
4. read_csv() function from the Pandas library can be used exclusively for reading CSV files.

**Question 3**

What will the following code print once executed?

```
my_list = []

for i in range(4):
	my_list.append(str(i) + str( len(my_list) ) )

print(my_list[3])
```

1. None
2. 2
3. 6
4. 33

**Question 4**

Which of the following statements is not true about scraping?

1. Scrapers broke over time, as websites change their structure.
2. Too aggressive (e.g. frequent) scraping may cause troubles for the website.
3. Scraped data may not be perfectly clean and need some additional processing.
4. Any data that can be publicly accessed can also be freely scraped.

**Question 5**

Which of the following regular expressions will correctly match the bold component in the following text:

"Dear students, please be informed that our midterm exam will be held on Monday, **June 19th, 15:30-16:45**."

1. \s([A-Z][a-z]+\s[0-9]{1,2}[a-z]{2}.+).
2. \s[A-Z][a-z]+\s[0-9]{1,2}[a-z]{2}.+.
3. [A-Z][a-z]+\s\S+.+
4. ,\s\S+\s\S+\s\S+



<h2 align="center">Part 2 – Short-answer questions (10 points)</h2>

METRIC is a Yerevan-based think-tank specialized in data-driven research and consulting. It has a website that can be reached at [http://metric.am/](http://metric.am/). You are asked to get data from this website using scraping techniques.

1. Please provide the link that you would check first before scraping METRIC's website.

2. Assuming the link you provided above shows the following information:
```
User-agent: sogou web spider
Disallow: /
```
What conclusions can you make regarding scraping after reading the information above?

3. The website continuously posts paragraphs from Wikipedia. The following is a copy from the page's HTML source of the part where a paragraph from Wikipedia was copied.
```
<p class = "wikipedia" id = "ranking_armenia">The economy of Armenia is ranked 132nd in the world,
with a nominal gross domestic product (GDP) of $10.561 billion per annum. It is also the 129th largest
in the world by purchasing power parity (PPP), at $25.329 billion per annum.</p>
```
Provide a Python code (using requests and BeautifulSoup), which will find the paragraph above and return its text to some variable.

4. Provide a regular expression that will find and return the 2nd ranking (129th) from the same text above. The expression must work even if the ranking changes significantly.

5. The paragraph is followed by a "Read more" text, which redirects to the original Wikipedia article page once clicked (the article page is: [https://en.wikipedia.org/wiki/Economy\_of\_Armenia](https://en.wikipedia.org/wiki/Economy_of_Armenia)). Provide the HTML source for the "Read more" text.

<h2 align="center">Part 3 – Open-ended problem (10 points)</h2>

[www.tert.am](http://www.tert.am) is an Armenian general-purpose online newspaper. The very first page has a table-like component in the bottom, which presents the news feed: hyperlinked titles of all published news in a day (see screenshot below).

![img](http://i67.tinypic.com/288cirl.png)

The inspected HTML source for this component of the page looks like this:

![img](http://i64.tinypic.com/qno77r.png)

*Note: the first &lt;div&gt; is responsible for the whole table-like component, then each &lt;p&gt; and &lt;div&gt; inside provide the content in that component.*

Please, write down a Python code, which will go to [http://www.tert.am/am/](http://www.tert.am/am/), find this table-like component and get from there the date (not time), the title and the link of each separate observation (i.e. published news), save this information in a JSON format and save the file into a JSON file. Please, provide careful explanation of all the steps you would take before, during and after writing this scraper code. Please, provide reasoning/explanation behind all components of your code (e.g. what each component is doing). You may provide it as Python comments or as a separate paragraph.