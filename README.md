#Cuisine 'n COVID19
#Restaurants map in Orange Countyin COVID19 situation

Stories: 
	 
	 1. I want to look for restaurants within Orange County. What kind of services do they provide (outdoor/indoor seating, take out, delivery, curbside, social distancing, and disinfecting and sanitizing). I want to find a restaurant that matches my criteria within Orange County. 10 Days
	 Tasks:
	 a)Extract location information and names of restaurants from Twitter API 
	 b)Create queries for the different keywords(seating, take out, ...)
	 c)Create interface for user/diner to search for services based on keywords(search bar,sub pages)
         
	 2. As a diner, I want to find restaurants near me that are COVID compliant. How are restaurants maintaining a safe and COVID compliant environment? 3 Days
         Tasks:
	 a)Create additional queries, with keywords related to a restaurant being COVID compliant(from Twitter feed) 
	 b)Design functionality for user to be able to set search radius on the map. 
	 
	 3. I want to see what others have said about certain restaurants. 3 Days
	 
	 Tasks:
	 a)Extract data from Yelp API, to get information/restaurant reviews from the other diners regarding the restaurants in diners' queries
	 b)Create window within program specificially for Yelp, to store reviews/information about restaurants as they become available. 
         
	 4. I would like to see information on how restaurants have been impacted by COVID (How long have they been closed for? Are they currently open?) 8 Days
	 
	 Tasks:
	 a)Pull data from Twitter API, posts from restaurants that talk about their open/closed status during pandemic. 
	 b)Display relevant information(in clear and consistent manner for all restaurants) found in tweets in pop-up dialogue window when user selects a certain restaurant on the map 
         
	 5. How much seating is available at a given restaurant? 2 Days
	 Tasks:
	 a) Pull information about seating/seating capacity percentage from restaurants' twitter pages 
	 b) Allow for user to query just seating information when looking up a specific restaurant 
         
	 6. I would like to have the option to see restaurants that match my given criteria within a list. 2 Days
	 Tasks:
	 a)Create a separate results box within the program -- show restaurants that match criteria user has given
	 b)Sort results by which criteria item the user entered in first 
         
	 -----Milestone 1.0----------
	 7. I would like to see a login page. 3 Days
	 Tasks:
	 a)Create landing page with GUI interface using Flask
	 b)Create interactive username and password text fields
         
	 8. I would like to see a map of restaurants within Orange County. 7 Days
	 Tasks:
	 a)Embed arcgis web-map of Orange County, display all restaurants as pins on map
	 b)Create boundary for Orange county using arcpy code, drawing polygon on top of map
         
	 9.  I want to be able to access my account and save my searches and preferences. 10 Days
	 Tasks:
	 a)Create user profile page -- which shows user's preferences and searches
	 b)Create a user account list, data storage location which allows diners to find people they know
         
	 Iteration #1:
	 Be able to log into program, enter in username and password 
	 5 days -- 10 hours total
	 
	 Iteration #2:
	 Be able to view and interact with map that has partial functionality 
	 8 days -- 16 hours total 
	
	 Burn down chart:
	 see file in git repository 


Timeline: Creating map of restaurants in given area(s)
				  Creating program to point to map given certain criteria
				  Testing programming, fixing bugs
				

Concept: A website that allows you to look for restaurants currently open during the pandemic, what services are being provided, and how they are enforcing COVID regulations. We will filter out information from Twitter and Yelp posts and reviews to obtain information that is most relevant to our website's goal. We will create the necessary map using GIS, and create a program that points to a given location within that map using queries to extract information from Twitter using Twitter's API.


Stakeholders: Residents of Orange County- people looking for dining options within Orange County based on certain criteria (see above in Story).
	      Restaurant owners
	      Restaurant workers
	      Travelers to Orange County
	      People looking for employment
	      County + State health officials 


Team members: Miles Von Herrmann, Dominic Lee, C. Vanessa Reyes, and Tony Sookthai

