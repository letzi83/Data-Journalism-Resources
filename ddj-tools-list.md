# Data journalism tools list

Link to this page: [http://bit.ly/ddj-tools](http://bit.ly/ddj-tools)

"Do data journalists need to code?" is a question I often get. My standard reply: "You don't have to, but it makes it easier." 

For myself, I decided to learn how to code when I figured that my current skillset (together with all the tools out there) were not sufficient to realize the ideas I wanted to do. 

So my advice would be: Think of a precise project you want to do and learn the skills on the go! When you see your newly gained power in effect it's much easier and encouraging to learn more.

And in fact, with the tools available online and mostly free, you can already do quite a lot!

So here's what should be in a data journalist's toolbox:

## Speadsheet software
You will need some sort of speadsheet software, it can be [Excel](https://products.office.com/en/excel) or [Open Office](https://www.openoffice.org/) as a a free and open-source alternative or [Google Spreadsheets](https://www.google.com/sheets/about/) - it actually does not matter which one you use, they all have the same functions you need to work with data.

When learning to work with any tool really, the search engine of your choice is your best friend: You are very likely to run into problems and also very likely someone else has had the same problem before you, wrote his problem somewhere on the internet and some other person explained how to solve it. So whenever you feel stuck - ask the internet for help!

The most common features I used and teach in spreadsheet software are:
- simple functions (like min, max, median, mean)
- VLOOKUP
- filters
- conditional formatting
- pivot tables
- and the charting function

All of them exist in every spreadsheet software, sometimes they are called slighlty different or are placed in different locations in the menu, but that's already it. You haven't heard of those features before? Well, go, ask the internet! ;)

### Cheat Sheets
- [Overview of Excel functions](https://support.office.com/de-de/article/%C3%9Cbersicht-%C3%BCber-Formeln-in-Excel-ecfdc708-9162-49e8-b993-c311f47ca173) and a [detailed list of functions](https://support.office.com/de-de/article/excel-funktionen-nach-kategorie-5f91f4e9-7b42-46d2-9bd1-63f26a86c0eb?ui=de-DE&rs=de-DE&ad=DE)
- [Overview of various more comprehensive cheat sheets, tips sheets and how to guides](http://mjwebster.github.io/DataJ/) made and/or compiled by [MaryJo Webster](https://twitter.com/MaryJoWebster), data journalist at the Star Tribute and ddj educator.

## Tools to clean data
If you have a speadsheet software, you already can do some data cleaning with that. For example using find+replace to get rid of unwanted blank spaces or quotation marks or thousand separators in order to make it recognize a number as an actual number (thus allowing you addition, substraction etc) instead of as a string.

However, sometimes data too messy for the spreadsheet software to handle; for example when you have a date that is formatted like `(MM/DD/YYYY)` but you want it to be `YYYY-MM-DD`. Find and Replace won't be of much help for that. Instead you need a 

**Text Editor**
This does not refer to the "Text Editor" preinstalled, but to a software like [Sublime Text](https://www.sublimetext.com/) or [Atom](https://atom.io/). Why? Because they are capable of searching for something called **Regular Expressions** (abbreviated: `.*`). It's like a secret language because letters, numbers and signs are encoded in symbols like `D` or `s` and thereby allows you to search for patterns and alter them. Like every secret language you have to put a little bit of effort into learning it, but then it's magical, because it allows you to perform the above task in less than a minute! There are multiple Regex manuals online - I often used [this list](http://www.rexegg.com/regex-quickstart.html) and [this list](http://www.petefreitag.com/cheatsheets/regex/) or this [cheat sheet](https://www.cheatography.com/davechild/cheat-sheets/regular-expressions/) for reference, but there are also tools letting you [practise regex online](https://regexr.com/). After some practice (just one project where you do lots of it) you'll know it by heart.

Another use of text editors is that they allow you to save files in different encodings like `utf-8` or `latin-1`; rule-of-thumb: whenever letters look weird (replaced by % or ~ or ?) you probably ran into an encoding issue and should try saving that file with another encoding.

**Open Refine**
Sometimes data cleaning is not about date formats, but you have a list of names like `Google, GOOGLE, gOOgle` or addresses that use different ways of typing the same information. You could do a lot of find and replace, but you can also use Open Refine, which recognizes similarity in data, groups them and asks you what your preferred output spelling version would be. It can also do some more analysis and again, there are many manuals on how to use it out there.

## Tools to find or gather data
If you don't have data for your project yet, you of course go search for it. 

When doing that [Google Advanced Search](https://www.google.com/advanced_search) is your best friend (or any other search engines with the following operators). Because in addition to typing your search terms and the word data in front of it, it lets you add `filetype:xls` or `filetype:csv` and it will only search for files of this type. This benefit is its disadvantage at the same time, because if your data is stored in a pdf file it won't be found in a `filetype:csv` search. So make sure to search with and without `filetype`. Also useful is the `site:` operator that only searches for results under the url you put after that operator.

Note that Search Engines do not index what is inside a database - so instead you have to search for a database then go to its webpage and search for adequate files there.

Sometimes the data you want or need is not there in a spreadsheed, but maybe hidden in a pdf or as a table imprinted on a website. Then it's time for **Scraping**. 

**Scraping from Websites**
When you don't know how to code, there are some options that help you do the job. For example Browser-Plugins like [Table2Clipboard](https://addons.mozilla.org/en-US/firefox/addon/dafizilla-table2clipboard/). Another option to scrape websites you can use the google spreadsheet pluging [import.IO](https://www.import.io/post/updated-bulk-extract-data-using-google-sheets/). If none of these do work, you have to step up and learn a programming language like Python or R to scrape more complex pages. Here's a [useful tutorial](https://data-lessons.github.io/library-webscraping/) starting at the very basics.

**Scraping from PDFs**
If you have a nice table, but it's imprinted in a pdf, you can use [Tabula](http://tabula.technology/) or a web-based alternative - for all of you who don't have admin-rights on their work-computers - [CometDocs](https://www.cometdocs.com/) to free your data! 

## Tools to visualize data

As you can see, we talked a bunch about finding and cleaning data, before we now come to the "fancy" visualization part. And this is reality! The actual visualization is just a small part of the ddj workflow, most of your time you will run into problems and try to fix them. 

If you managed to not give up during that phase, you can finally move on to the next one: Visualize your data! In fact, that's also part of the analysis, because [Anscombe's quartet](https://en.wikipedia.org/wiki/Anscombe%27s_quartet) and because we are way better in perceiving patterns in a visual form rather than in a table. 

There are many tools out there, all with various functions:

- [Datawrapper](https://www.datawrapper.de/) is probably a good point to start
- [Tableau](https://www.tableau.com/) is what I would recommend you to use if you feel Datawrapper does not give you enough options

**Mapping**
- [QGIS](https://qgis.org/en/site/forusers/download.html) is an open source mapping tool with myriads of customization options -- [here](https://gcgruen.github.io/teaching/qgis/index.html) you can find a tutorial I wrote on how to make a chorolpeth map in QGIS
- [Carto](https://carto.com/) is what I use when I teach mapping. They recently did a relaunch and the community is kind of mixed over whether that was a good or a bad move. Datawrapper and Tableau both offer the option to make maps as well, but Carto still has some more features. 

Of course, there are more, like [Highcharts](https://www.highcharts.com/), [Mapbox](https://www.mapbox.com/) and [Leaflet.js](http://leafletjs.com/) for example. But the above ones are definitely good starting points.

## Design Tools
The above tools all include the option to customize a chart's design. If you want to go beyond the offered options, I would suggest using a **design software** like [Adobe Illustrator](http://www.adobe-students.com/de/creativecloud/buy/students.html?sdid=KKTIB&mv=search&s_kwcid=AL!3085!3!186073542703!b!!g!!adobe%20illustrator%20creative%20cloud&ef_id=WVIVLQAAAHNc5D2H:20180121181424:s) or [Inkscape](https://inkscape.org/en/) as a free and open-source alternative.

If you already know about the usage of colors and just want to find a suitable custom **colour palette** for your project, check out [colorbrewer2.org](colorbrewer2.org) or [coolors.co](coolors.co) or. If you are starting from scratch, you might want to read [this blog post](https://blog.datawrapper.de/colorguide/) by Lisa Charlotte Rost about the importance and usage of colors first - it also comes with a lot of recommendations for different tools to help you make good choices.

In my daily work I found some **Browser-Plugins** to be really useful for design tasks:
- [WhatFont?](https://chrome.google.com/webstore/detail/whatfont/jabopobgcpjmedljpbcaablpmlmfcogm?hl=en) Identifies font on a webpage
- [Colorzilla](https://chrome.google.com/webstore/detail/colorzilla/bhlhnicpbhignbdhedgjhgdocnmhomnp?hl=en) picks colors from webpages
- [MeasureIt](https://addons.mozilla.org/en-US/firefox/addon/measureit/) virtual ruler meausring specs of elements on a page

## More

Of course I am not the first one to write down a list of data journalism tools. There are maaaaaany others who already did this, in a way more beautiful way. For example:

- [Data Journalism Tool Collection](http://journocode.com/data-journalism-tools/) by [Journocode](https://twitter.com)
- [Data Journalism Tools](https://datajournalism.tools) with a task-based search function by [Yael de Naan](https://twitter.com/yaeldehaan), [Renée van der Nat](https://twitter.com/mechanicalangel) and [Winny De Jong](https://twitter.com/winnydejong) 
- [Dataviz Tools](http://dataviz.tools/) by [Carl V. Lewis](https://twitter.com/carlvlewis)

Besides these collections, there are **websites naming essential tools**
- the [Knight Science Journalism Tracker](https://ksj.mit.edu/data-journalism-tools/) 
- the [Data Journalism Handbook](http://datajournalismhandbook.org/1.0/en/delivering_data_7.html) 
- the [Global Investigative Journalists Network](https://gijn.org/2016/04/25/a-data-journalism-experts-personal-toolkit/)
- the [Knight Center of the University of Texas](https://knightcenter.utexas.edu/blog/00-14184-6-more-digital-tools-your-data-journalism-kit)
- the [European Journalism Centre](http://datadrivenjournalism.net/resources)  






##### Usage and license
*Compiled by [@giannagruen](twitter.com/giannagruen).* 
*Feel free to use, share, edit these collections for non-commercial use under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) license. For purposes not covered under that license, please feel free to get in touch via the above mentioned email.*
