# IST-303-Team-B-Project
***
## Part A
---

## Product: Cuisine 'n COVID19
Orange County Restaurant COVID19-compliant
Restaurants map in Orange County in COVID19 situation

**Concept:** A website that allows you to look for restaurants currently open during the pandemic, what services are being provided, and how they are enforcing COVID regulations. We will filter out information from Twitter and Yelp posts and reviews to obtain information that is most relevant to our website's goal. We will create the necessary map using GIS, and create a program that points to a given location within that map using queries to extract information from Twitter using Twitter's API.


### Team member:
Dominic Lee, Vanessa Reyes, Thawachsorn Sookthai, Miles von Herrmann


### Stakeholders:
* Residents of Orange County- people looking for dining options within Orange County based on certain criteria (see above in Story).
* Restaurant owners
* Restaurant workers
* Travelers to Orange County
* People looking for employment
* County + State health officials 

### Research:

[![N|Solid](https://i.ibb.co/xF6pQzb/SafeDine.png)](https://www.ocbc.org/safedineoc-grantrecipient/)

The County of Orange announced on August,6 2020 that the launch of a new SafeDineOC COVID-Safe Restaurant Campaign to incentivize Orange County restaurants to follow California Department of Public Health (CDPH) guidance to prevent the spread of COVID-19.

Restaurant owners may apply for a $1,000 grant per Orange County restaurant location for taking steps to create a COVID-safe environment for their customers and employees. The grant will reimburse restaurants for purchases of personal protective equipment including face masks, cleaning products, employee training and costs for physical distancing of tables and chairs, as examples.

The SafeDineOC campaign is sponsored by the County of Orange and managed by Orange County Business Council (OCBC), which will handle intake and approval of all restaurant applications as well as disbursement of the $1,000 grants to restaurant owners. Through its comprehensive database of restaurants, the OC Health Care Agency will ensure the promotion of the campaign to all restaurant owners in the County.

Restaurants that apply and are approved will be added to a list of COVID-safe eateries organized by city that will be available to consumers on the SafeDineOC website. This online resource will enable the public to see which restaurants offer a safe dining experience in Orange County

“Maintaining consumer confidence in the restaurant industry is critical to helping businesses stay afloat during these challenging times,” said Supervisor Lisa Bartlett. “When customers visit a restaurant, they want to be confident that it is clean and in compliance with County health and safety guidelines,” said Bartlett. “The safety and protection of restaurant workers, and the customers they serve, is paramount to stopping the spread of COVID-19,” she said.

Finally, the OCBC (Orange County Business Council) launched the list the forefront of safely serving Orange County at https://www.ocbc.org/safedineoc-grantrecipient/

[![N|Solid](https://i.ibb.co/Qv60Qc3/Logo-2.png)](https://orangeeco.envisionconnect.com/#/pa1/search)

The Orange Health Care Agency has published the list of restaurants which has been joined the food inspection campaign. The list is contained upto 13,000 restaurants across the county. Our group extract the list which includes restaurants'name and address.



### User Stories (estimate of completion times) and development priority:
**As a user:**
 1. I want to look for restaurants within Orange County. What kind of services do they provide (outdoor/indoor seating, take out, delivery, curbside, social distancing, and disinfecting and sanitizing). I want to find a restaurant that matches my criteria within Orange County.
         
2. As a diner, I want to find restaurants near me that are COVID compliant. How are restaurants maintaining a safe and COVID compliant environment?
	 
3. I want to see what others have said about certain restaurants.
         
4. I would like to see information on how restaurants have been impacted by COVID (How long have they been closed for? Are they currently open?)
         
5. How much seating is available at a given restaurant?
         
6. I would like to have the option to see restaurants that match my given criteria within a list.
         
7. I would like to see a login page. 
         
8. I would like to see a map of restaurants within Orange County.
         
9. I want to be able to access my account and save my searches and preferences.
       
 
### Process:
Timeline: 
* Creating map of restaurants in given area(s)
* Creating program to point to map given certain criteria
* Testing programming, fixing bugs


### Class Presentation Slides:  
Project proposal : Project Requirements Part A

[![N|Solid](https://i.ibb.co/j686cQY/googleslide.png)](https://drive.google.com/file/d/1pJJzOb0ccUWlm0MDcwRktVupkhMgKlMe/view?usp=sharing)

Project proposal : Project Requirement Part C

[![N|Solid](https://i.ibb.co/j686cQY/googleslide.png)](https://drive.google.com/file/d/1I9grItT5u3tvy1lVU38PCQDL98VdU1Ru/view?usp=sharing)
***  

## Part B
---

### User Stories decomposition into tasks with team member allocated:

1. I want to look for restaurants within Orange County. What kind of services do they provide (outdoor/indoor seating, take out, delivery, curbside, social distancing, and disinfecting and sanitizing). I want to find a restaurant that matches my criteria within Orange County.  
*10 Days*  
**Tasks:**  
a) Extract location information and names of restaurants from Twitter API.  
b) Create queries for the different keywords(seating, take out, ...).  
c) Create interface for user/diner to search for services based on keywords(search bar,sub pages).
         
2. As a diner, I want to find restaurants near me that are COVID compliant. How are restaurants maintaining a safe and COVID compliant environment?  
*3 Days*  
**Tasks:**  
a) Create additional queries, with keywords related to a restaurant being COVID compliant(from Twitter feed).  
b) Design functionality for user to be able to set search radius on the map.  
 
3. I want to see what others have said about certain restaurants.  
*3 Days*  
**Tasks:**  
a) Extract data from Yelp API, to get information/restaurant reviews from the other diners regarding the restaurants in diners' queries.  
b) Create window within program specificially for Yelp, to store reviews/information about restaurants as they become available.  
         
4. I would like to see information on how restaurants have been impacted by COVID (How long have they been closed for? Are they currently open?).  
*8 Days*  
**Tasks:**  
a) Pull data from Twitter API, posts from restaurants that talk about their open/closed status during pandemic.  
b) Display relevant information(in clear and consistent manner for all restaurants) found in tweets in pop-up dialogue window when user selects a certain restaurant on the map.  
         
5. How much seating is available at a given restaurant?  
*2 Days*  
**Tasks:**  
a) Pull information about seating/seating capacity percentage from restaurants' twitter pages.  
b) Allow for user to query just seating information when looking up a specific restaurant.  

6. I would like to have the option to see restaurants that match my given criteria within a list.  
*2 Days*  
**Tasks:**  
a) Create a separate results box within the program -- show restaurants that match criteria user has given.  
b) Sort results by which criteria item the user entered in first.   
         
**-----Milestone 1.0-----**
 
7. I would like to see a login page.  
*3 Days*  
**Tasks:**  
a) Create landing page with GUI interface using Flask.  
b) Create interactive username and password text fields.  
         
8. I would like to see a map of restaurants within Orange County.  
*6 Days*  
**Tasks:**  
a) Embed arcgis web-map of Orange County, display all restaurants as pins on map.  
b) Create boundary for Orange county using arcpy code, drawing polygon on top of map.  
         
9.  I want to be able to access my account and save my searches and preferences.  
*10 Days*  
**Tasks:**  
a) Create user profile page -- which shows user's preferences and searches.  
b) Create a user account list, data storage location which allows diners to find people they know.  
         

### Iterations for Milestone:
**Milestone #1**
- Be able to log into program, enter in username and password 
- Be able to view and interact with map that has partial functionality 


### Velocity
### * Milestone 1
There are 3 user stories in Milestone 1
Days needed = 19 days | Assume that 4 working hours per day | 4 developers --> 1 hour per team member

| Task No. | Task | Days required | Hours required |
| ------ | ------ | ------ | ------ |
| 7a | Create landing page with GUI interface using Flask. | 3 | 12
| 7b | Create interactive username and password text fields. | 4 | 16
| 8a | Embed arcgis web-map of Orange County, display all restaurants as pins on map. | 3 | 12
| 8b | Create boundary for Orange county using arcpy code, drawing polygon on top of map. | 3 | 12
| 9a | Create user profile page -- which shows user's preferences and searches. | 3 | 12
| 9b | Create a user account list, data storage location which allows diners to find people they know. | 3 | 12
| | Total | 19 | 76 (19x4)

It is complicated to calculate base on task completed, then we calculate base on sum of working hours used vs number of day left.
We have calculated the velocity as below:
* Sprint start date: 7-Oct
* sprint end date: 2-Nov
* working days:	19
* team size: 4
* work hours per day: 1
* total available hours: 76
* average daily available hours: 4
* average productivity:	80
* productivity hours: 60.8
* average daily productive hours: 3.2

### Burn Down Chart:
We have created the burn down calculator to input the working hours for each developer.
Please follow the link https://bit.ly/31q50o7
(Only CGU member with this link can access, but only our team can edit)

[![N|Solid](https://i.ibb.co/C2F1Zwr/GraphM1.png)](https://bit.ly/31q50o7)


### Stand Up Meeting:
* Meeting #1 Sep 13: Brainstorming, initiate the project, sharing background and identified user stories
* Meeting #2 Sep 15: Finishing draft of pitch, user stories, working hour estimation, velocity and user stories
* Meeting #3 Sep 23: Update progression and challenges
* Meeting #4 Oct 06: Update milestone#1 for project requirement A
* Meeting #5 Oct 13: Update progression and agree to use Flask
* Meeting #6 Oct 16: Update progression and challenges, brainstorming to solve the problems
* Meeting #7 Oct 21: Update progression and challenges, the list of restaurants in Orange county
* Meeting #8 Oct 28: Update progression and challenges, pin map, username / password database
* Meeting #9 Oct 31: Update progression and challenges, pytest and installing the packages

### Functional and Test Code:
* Test load URL index
* Test load URL dashboard
* Test login
* Test signup

### Environment to run application
* Python 3.7
* Pip
*
*
To be advised


### Run Application Command
How to run website:

1) Save Project folder to Desktop on computer
2) Navigate to Project folder within terminal 
3) Run the following on Terminal:
	$ python3 Cuisine.py
	$ export FLASK_APP=Cuisine
	$ export FLASK_ENV=development
	$ flask run
4)Copy URL(http://127.0.0.1:5000/) and paste into web browser 
