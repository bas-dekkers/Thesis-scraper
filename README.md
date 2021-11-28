# Thesis-scraper
In this repository can 2 python scripts be found. These scripts have been used to collect additional data for my thesis. 
In the text below I will shortly explain what each scraper does. 

## Scrapers
### Thesis_scraper_creators 
This webscraper visited per channel ID’s two pages and merged the information it scraped from those two pages at the end. The first page it visited was "https://www.youtube.com/channel/" + channel ID + "/videos". On this page the scraper kept scrolling down to the bottom of the page to load videos until the moment when there are no more videos to load, then it calculates the number of videos present and saved that number. Furthermore, the channel ID was scraped to be able to merge the separate csv files in the end of the scraper, but also to merge it with the initial dataset. The second page that was visited was "https://www.youtube.com/channel/" + channel ID + "/about" and from this page the creator’s name, number of subscribers, total number of views, the date account was created and channel ID were collected. All this information could be scraped from the page without adding extra functionalities. 

### Thesis_scraper_comment_section
This webscraper visited every video and scrolled down till all the comments were loaded. When all the comments were loaded it counted the times the creator liked a comment (give it a heart) or responded to a comment. Since YouTube has a special button when a creator responded or when creator liked a comment the times those buttons appear were counted. See picture below for the special buttons.
![image](https://user-images.githubusercontent.com/79585712/143772716-f93e42eb-01bd-452a-a287-2a82bccbc095.png)

## Analysis
### R code
To analysis this data and the initial provided data an R script was written. 
This script isn't cleaned yet, but will be uploaded soon!
