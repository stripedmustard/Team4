## Team 4
<!DOCTYPE html>
<html>
<body>
	<a href="https://github.com/stripedmustard/Team4/blob/master/Dean/Dean.md">Dean</a> 
	<a href="https://github.com/stripedmustard/Team4/blob/master/Grace/Grace.md">Grace</a> 
	<a href="https://github.com/stripedmustard/Team4/blob/master/Jacob/Jacob.md">Jacob</a>
</body>
</html>

## Prototype
<html>
<body>
	<a href="https://www.youtube.com/watch?v=KMXrVrTFd3Y">Prototype Test 1</a>
</body>
</html>

## Architecture Presentation
<html>
<body>

</body>
</html>



## Daily Activities
**_1/18/19_**
Today we met with Ryan, as a group, for the first time to go into more detail about the project. We went into specifics about the Blog
Bot. Ryan mentioned that our Blog Bot must not publish the posts, but should send the posts to him. According to the Kentucky Bar Law
Association, only lawyers can create such posts to their blog. Ryan said that the Blog Bot should send an email of the drafted post to
him. Ryan said that he would prefer a range of five hundred to one thousand words on each blog post. In the middle of the meeting, he
introduced us the Lonnie, their web guru. Lonnie mentioned that he is familiar with the logistics of our project and said that we can
contact him if we have any questions or concerns. 


**_1/24/19_**
Today, we all met on campus and discussed how each of us would start the project. Dean started the meeting by conducting research on creating an online Wordpress plugin. Currently, Jacob is in a Web Crawling class with Dr. Brent Seales. He talked about bringing his knowledge of web crawling to help us with the project. Jacob contined doing research on the Web Crawler, more specifically on how to deelop the Web Crawler.

**_1/29/19_**
Today, we met at Dean's place to continue progress on our project. In the beginning of our meeting, Dean researched how to create an
online Wordpress plugin. In our first meeting with Ryan, he mentioned that he would give us access to a Wordpress plugin, but we ended
creating a local one on Dean's computer. Jacob helped by looking up how to create a Wordpress account. Grace started to research
important keywords and phrases for the articles that we will create. Grace started off with the keyword DUI, since Ryan mentioned that
he would like to focus more specifically on DUI's. Jacob did research as well and stumbled upon findlaw.com. This website has content
for just about any legal topic that you could think of. In addition, it helps users find lawyers from various cities and states. When
searching the term DUI on findlaw.com, we found our client, Cooley Iuliano Robey, PLLC, on the list of Top Lexington DUI Lawyers in
Lexington, KY. This was an interesting thing to discover, especially at the beginning of our project. Grace found various websites 

**_2/1/19_**<p>
Met with Ryan and Lonnie via Google Hangouts and discussed:<p>
- Page Optimzer Pro, an application that will help us tremendously
- How to get high on Google Rankings
- Potential faults with the Blog Bot, regarding potential issues that could hurt the Google ranking of a website

**_2/6/19_**
Today, we met and talked about creating the team website. Grace agreed to create the website, montior the website and update it with the current word count of each member as well as 
- Talked about creating the team website
- Updating the Web Crawler application

**_2/12/19_**
Today we created a website that will provide the details of all our team meetings, hold each team member's developer notes, and
discusses the progress we have made with our project throughout the semester. We tested the Web Crawler and it was able to find articles
relating to our keywords. Lastly, we tried out Page Optimizer Pro for the first time. Lonnie recommended that we take a look at Page
Optimizer Pro because he believed it would help us understand how to improve the Google rankings of the Wordpress articles. 

**_3/1/19_**
Early this morning, we met with Ryan to talk about Page Optimizer Pro. This was the tool that Lonnie said would help us get a start on
our plugin. In addition, we gave him an update on our project. Currently, our prototype consists of the Web Crawler and an offline
Wordpress plugin. Our Wordpress plugin can find articles relevant to the keyword provided, copy the article and publish a copy of the
article to the offline Wordpress site.

**_3/4/19_**
- Met at Presentation U to review presentation that will be presented on Wednesday March 6
- Presentation was critiqued by Presentation U tutor
- Listened to suggestions made by Presentation U tutor
- Practiced Architecture Design Presentation

**_3/5/19_**
Today we had a meeting to practice presenting our Architecture Design Presentation. 

- Meeting to practive Architecture Design Presentation
- Met with Ryan to show prototype of project

**_3/6/19_**
Today, we presented our Architecture Design. In it describes the functions of the Web Crawler, Scraper, Plugin and Database. We provided a timeline that projects each step that it takes to create the Blog Bot. In addition, we added some strech goals that we would like to accomplish if the time permits. 

**_3/19/19_**
Jacob and Dean met with Ryan at his office and presented the prototype. They had some difficulties presenting it, so Dean created a
video that walks through our Wordpress plugin.

**_4/3/19_**
We met today and talked about what each person will be working on moving forward. Grace will be working on the database. She will use a
Lamp server which should be compatible with our Web Scraper. In our database, we will save the articles that were used to generate the
article so that when the web crawler is looking for articles, it will avoid articles that we have already discovered. Grace mentioned
that she was having difficulty logging into her Mutilab account. However, she mentioned that she will find a way to get access to her
account and start the process of creating a LAMP server. The LAMP server will hold the list of pages that we need to fetch and the list
of pages that we have already fetched. That way, we avoid looking for content that we have already discovered. If we still have time, we
would like to add the date that the article was fetched to the database. Jacob mentioned that we need an adjacency list, where each URL
followed by the thing that the URL points to on its page. Dean stated that he will work on getting the Wordpress plugin to call the
Script. Then, we talked more about the database. We mentioned that the database will save the URL of the webpage of the fetched articles
so that we not only know have a record of discovered article, but we can retract back to the webpage if needed be. We all agreed that
the difficult task is figuring out how to store Python dictionaries into a SQL database. Dean mentioned that he was made LAMP servers in
the past and that we could probably use a LAMP server for our project. Grace plans to work on creating the LAMP server once she figures
out what is going on with her Multilab account. Dean suggested that Grace work on the LAMP Server on his desktop and Grace agreed that
would be a good solution if she is not able to get her account working. Someone brought that they would like to have a sample of the
database ready before we visit Ryan. As of now, we are still figuring out a time that we all can meet. Jacob created a list that
describes all of the things we need to do as of now. Jacob also went more into detail about the adjacency list, entailing what the
adjacency list will do as well as why it is needed. Dean made up a list of things that he plans to do within the next few days. He
mentioned that he plans to create a plugin settings menu that calls Jacob's script and then saves to draft. Once again, we brought up
the database. We wanted to figure out if it is possible to store a Python list or dictionary in a database. Shortly after, we concluded
the meeting.

**_4/7/19_**
On Sunday, Grace met with Dean at his house to create a LAMP server on Dean's virtual machine. They had some issues with permissions but
were able to work around that. Finally, they were able to install mySQL and eventually, the LAMP Server was created. Grace will be
working on the database on Dean's virtual machine. Grace will start off by creating a database with sample entries for the meantime. She
created an Article, Keyword, and Website table. The Article table holds the Article Name, an auto-incremented Article ID, and the
Website URL. The Keyword table has the Keyword, the Article ID (generated in the Article table), 

**_4/8/19_**
Today, we created a settings page that calls the Script in order to create a new article and saves the article as a draft. 

**_4/15/19_**
Today, we met and discussed what other parts of the projects that we need to work on. For the demo of the Coding Assigment Presentation, we would like to use Ryan's FTP permissions to install the plugin and the Python script. We logged into Ryan's FTP and discvovered that it did not work. After doing some thinking, we concluded that, for the presentation, we will provide screenshoos of the local Wordpress plugin. Grace mentioned that she would like to get the Web Crawler and Database integrated. Even though our parts are completed individually, we have yet to bring all the Web Crawler, Wordpress plugin and database together. It is not a simple task, but we hope to complete this during the weekend. 

**_4/26/19_**
Today, we integrated the Wordpress Plugin with the Web Crawler. We are still trying to integrate the Wordpress Plugin with the database. 


Grace Word Count: 1573 words
