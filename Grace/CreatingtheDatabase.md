## Creating the Database


<!DOCTYPE html>
<html>
<body>

Before creating the database, I brainstormed, thinking of attributes and entries necessary for our project. We made a sample table that we
presented on our Architecture Presentation (The Database Description slide) as well as some Entity Relationship diagrams. I started off by
creating an Article table. Originally, I thought that I could just auto-increment the ID of each Article added to the database without the
name of the article. Later, I thought it would be beneficial to add the attribute "Article Name" for to the database for stylistic
purposes. In addition, it would be beneficial to have the article name in the database.  Inspired by our original table, I added the 
attributes Source and HTML Page. At first, I added the keyword to the table, but it made more sense to create a table specifically for our
keywords. I created a Website table that hold the URL and the title of the webpage. I wanted to create a Fetched attribute for the Article
table that tells the user whether we have downloaded and created a blog post out of the article. Because I had issues creating the Fetched
attribute in the Article table, I just created a Fetched table with a Fetched attribute for the meantime. 

On Monday April 15, we met together to talk about finalizing the project. 
