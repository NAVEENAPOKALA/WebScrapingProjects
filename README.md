# WebScrapingProjects
Scraping the Web Pages using Beautiful Soup, Selenium and Request Library

Problem Statement : 

   1) Scraping the list of page names and their respective urls of popular communities, gaming, sports, TV, Travel, Health and Fitness, Fashion categories on reddit home page
   2) Scraping all the individual pages and collecting information like description, created date, total no of followers or subscribers, total no of people that are online
   3) Saving the collected data into a CSV.
 
Function Descriptions :

   1) get_inner_div_tags function takes the outer_div_tags as input and returns the entire 'div' component of all pages like AskReddit,NoStupidQuestions and is stored in list         component called inner_div_tags
   2) get_a_tags function takes inner_div_tags as input and returns the entire 'a' component that id having page title and page href of all pages and is stored in list               component called total_a_tags
   3) get_topic_details function takes total_a_tags as input and returns pages name , urls and is stored in topic_names, urls attributes
   4) get_topic_infos functions takes urls as input and inturn calls another function get_topic_info which returns description, created date, total no of followers or
      subscribers, total no of people that are online of individual pages
   5) get_topic_infos appends the individual page details and returns the list components topic_description,topic_members,topic_online,topic_createddate
