---
published: true
tags:
- Side Projects
- Reflections
---

Yesterday, I buckled down and thought it was finally time to get something done, so I thought I start work on helping C out with her capstone. Previously, I had thought of certain ways to get it done, but procrastinated so much on it I hadn't actually tried doing it due to the workload. With an entire day in front of me, I could finally put in some hours. 

One part to her project entailed scraping data about Christie's auctions, and she required the following: The artist, the title of the work, price realised, the low and high estimate, and the lot number. I had use an auction as a sample, and derive some rules to scrape the data off the page. The first thing I realised is that the lots load dynamically and can't be scraped off the page immediately. Furthermore, the information I required were on another page so I couldn't just get the data off the same page. 

A quick search on google shows many scraping packages available, the most basic ones being BeautifulSoup and lxml, which are able to parse the DOM and retrieve text with ease. Then there are more high-level packages such as Scrapy and Selenium, which adds more functionality to BeautifulSoup and lxml. I thought of using Scrapy first, and used their Spiders to parse the webpage. However, I ran into the problem of getting the data loaded dynamically. One thing I did appreciate was the Scrapy shell, which I could use to debug my scraping scripts - whether I was getting the XPath or CSS selectors correct or not. This gave me the confidence to know that it wasn't my requests that were faulty, but that it was the data being loaded with some delays. 

Now, what to do about the delayed loaded data? I thought of using Selenium, as it gives me complete control over the browser. It allowed me to load the page, wait for it to fully load, and then I had to click on a 'load all' button to load all the lots as some of it wasn't displayed. Then, I realised I could also use Selenium to grab all the links to each lot and save them in an array. I then passed the array to my Scrapy spider which went through each link and grabbed the relevant details I needed. 

This combination of Selenium and Scrapy certainly worked, and I tried it out on Sothesby's website, but unfortunately, they are smart and blocked all sorts of scraping on their website. I knew this as I ran into a 400 (Forbidden) error, and checked their website's user policy, and certainly it was there. 

Finally, I had to package the scraper for C to use, which made me wonder how I could have packaged it better. I've never written code that other people had to download, so I am wondering if I could have made like a little applet that downloaded all the required dependencies for her, and wrapped the entire code up so she can only give her own input. But, I guess that would have been a lot of time where she could just do it following the instructions I gave her. It was then, that I also realised how much I rely on Terminal, where someone else may not have the same experience too. I guess I'm grateful for my coding education? Hahahaha.

All in all, I think it was a good day learning how to scrape websites properly, and if you want to check out the code it's on my github @evanma92!