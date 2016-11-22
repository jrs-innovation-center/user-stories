[Home](/)  |  [Data](/lunchit/data)

# LunchIt! User Stories

## Overview

### Elevator Pitch

A progressive web application (PWA) that takes the hassle out of deciding where to eat for lunch.  Simply shake your phone and LunchIt! will pick the best place to eat lunch based upon preferences and history. Easily access restaurant information and create reservations.

### High level Process

- Create Circle - Create and mange your circle of lunch friends.
- Discover - Integration with OpenTable makes it easy to discover the best places to eat. Built in maps make it easy to find the coolest new places.
- Pick your favs - Build and manage your list of favorite restaurants.
- Shake - Shake the app to start a session. Let LunchIt! pick the best place to eat based upon your circle's preferences.
- Rate - LaunchIt knows when its time to rate your dining experience.  Your preferences are saved to your favs for future LunchIt! sessions.

## Create Circle

As a user, I often eat with the same group of people from work.  I want to define a circle of friends in order to make the process of deciding who is going to lunch easy. I desire an easy step by step process where I:

- Provide a name for the circle, such as "Co-workers" or "Family".
- Search for friends in the Friends Directory and once found, add them to the circle.

See **Manage Circle**.  

## Manage Circle

As a user, I want to manage the friends in a specific Circle.  I want to see a list of my Circles. After selecting a circle, two lists appear:

- A listing of existing friends that are in the selected circle.
- An alphabetical listing of friends that are not in the circle.

Checking a name in the circle, moves the name outside the circle.  Checking a name not in the circle, moves the name in the circle.

## Select Circle as Default

As a user, I want to designate a specific circle as my default in order to streamline the process of activating a LunchIt! session.

## Search OpenTable Restaurant data

As a user, I desire the ability to find a restaurant by:

- zip (http://opentable.herokuapp.com/api/restaurants?zip=29466)
- price (and zip) (http://opentable.herokuapp.com/api/restaurants?zip=29464&price=2)
- name  (http://opentable.herokuapp.com/api/restaurants?name=red%20drum)

List the search results that include the restaurant name, address, and price rating (1-4).  Selecting an item on the list displays an image of the restaurant, the location on a map, and restaurant name, address, and price.

Once I find a restaurant, I want the ability to create a reservation using OpenTable.  

## Pick My Favs

As a user, I wish to build a list of my favorite restaurants.  I desire the ability to search for a restaurant and save it as a favorite.  

## Activate LunchIt! Session

As a user, I want the ability to easily decide on the best restaurant for lunch by simply shaking my phone or clicking a button.  The system should suggest the best option based upon my preferences, friends preferences and session history.  If I don't like that option, I can elect to view additional restaurant options.  I want to pick the best option and save it to my session.

## Check In to Restaurant

As a user, I want the app to know my current location and know when I am at the restaurant.  I want the application to prompt me to:

- Rate the restaurant
- Mark or it as a favorite in my preferences
- Block the restaurant in my preferences

## Rate Restaurant During LunchIt! session

As a user, I want to rate a restaurant during my session by providing a rating of 1 through 4.  The system will save the rating for my current session and save the rating for the restaurant in my preferences.

## Mark Restaurant as Favorites

As a user, while I am rating a restaurant, I can elect to save the restaurant as a favorite.  As a result the system will save the restaurant in my preferences.

## Block a Restaurant

As a user, there are certain restaurants that I do not like.  I desire the ability to search for a restaurant and add it to preferences as a blocked restaurant.  

## Send SMS to Friends

As a user, I want the ability to easily tell my friends where to eat lunch.  After activating a LunchIt! session, I want the ability to send a text to all the friends listed in my LunchIt! session.  

## Up-vote Restaurant within LunchIt! session

As a friend who is in a circle, I want the ability to open the current LunchIt! session that I am associated with and up-vote or down-vote a LunchIt! recommended restaurant and optionally provide a related comment.
