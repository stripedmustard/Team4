<!DOCTYPE html>
<html>
<body>
<p>  
Meeting 1/29
I began this meeting by researching how our group can install a staging site for wordpress on one of our Windows computers.
I then learned about WAMP, a Windows application for hosting Apache, MySQL and PHP  plugins.
After installing WAMP on my desktop, I had to setup MyPHPadmin and create a database
I created a database called "wordpress_db" and then installed wordpress using a .zip file from wordpress.org
I created a wordpress plugin named 'articatch' by simply adding a file 'articatch.php' to the /wp-content/plugins directory.

2/12/19
During this meeting I did a lot of research on Page Optimizer Pro. One of my goals was to figure out how the website's functionality worked.
I was assured when I realized that Page Optimizer Pro operated with the same logic as the Beautiful Soup API we had planned to implement.
Our plan was to use Beautiful soup to keep a counter of keyterms and related terms' occurance per each verious HTML tag (such as "<h1>,<h2>,<a>, etc)".
I did discover one shortcoming of Page Optimizer Pro. It seems to me that when the software was aimed at evaluating the Search Engine Optimization of a certain site, it would use the keyword statistics of comparison sites to do so. 
The problem being, if there wasn't any keyword data at all on the comparison sites, then the Page Optimizer tool would reprt false positives.
For instance, if the software didn't find any comparison websites at all, it would report that they had 0 occurances of the keyword. But in reality there was just 0 data.
An easy solution to this of course would be to simply check whether comparison data was availabe.


Meeting 4/3
During this meeting I did a lot of research over how I could construct our optimimum UI for the Wordpress plugin.
Me and my group mates created game plan for how to complete the final stretch of our project:
1. Create a plugin settings submenu, with a user interface that calls the program functions with the click of a button.
2. My second goal was to rewrite our wordpress shortcode to call jacob's python script.
It turned out that this goal was short-sighted, as my true task ended up being to get rid of the shortcode functionality altogether.
I didn't need to use Wordpress shortcodes because the plugin settings menu would be calling python scripts directly.
3. My third task was to verify our SSH credentials with Ryan. After some back and forth I got in contact with his dedicated IT team.
They sent me FTP credentials to the website server, but it turned out the site was actually secured with STFP.
This means that I'd need a private key to to access, which I was not able to receive.
4. My final task from this meeting was to help Grace with the database design. We hypothesized 3 data tables:
One for the keywords we'd be itemizing, one for the articles we've downloaded, and one for the websites we are crawling.
 

Meeting 4/11
Met with Grace to revise and implement our database tables.
The Keyword table will be the primarily accessed table, fetching Article ID's when the Wordpress plugin queries for a new article.
The Article table will be used to fetch the website URL, once an article ID has been selected
The Site ID table will be accessed at the end of each article query; its main purpose is to keep track of which articles have already been used before.
I set up a new virtualbox on my local machine and installed a new LAMP server. Grace built a new database on Phpmyadmin with our 3 tables.

Meeting 4/18
At this point Jacob had completed a new version of his python script, which is now taking urls to download from a neighboring JSON file.
 On this day my primary goal was to modify my plugin, which was currently calling an older version of Jacob's script that only read from a defined URL.
In total it took me 11 hours to solve the problem. At first I simply changed the script path from the old script to the new one. When this didn't work, I assumed it was a problem with Apache not having sufficient permissions.
I then tried using the absolute path rather than relative, changing the function from exec() to shell_exec(), moving the script to my root directory, and more desperate debugging attempts.
Finally I tried calling PHP function get_user() which revealed that I was using /wp-admin as www-data. So, I opened my local sudoers file and gave www-data full sudo power (a dangerous move).
Of course, that didn't work. After several hours I finally discovered that Apache had error log files. I opened them and found out that the .json dependencies for his script were not being found, as if they didn't exist.
I went into his plugin, baseArticleSelector.py and I changed the paths for articlesUsedAsBasesList.json and articleURLsToBeVisited.json- I appended /var/www/html/wordpress/wp-content/plugins/articatch to their paths.
This worked! I was now able to genereate a new article with each function call by using Jacob's python file to get new URLs.

Word count: 851
  
  </p>
</body>
</html>
