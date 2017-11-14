[Home](/) | [User Stories](/lunchitapp/)

# LunchIt Data

## My Restaurant Preferences

- My Restaurant Preferences ID  - Primary Key. Represented as either an `_id` key in CouchDB.  `ID` table column MySQL database.
- Restaurants
  - Restaurant ID  
  - Preference Type (Favorite or Blocked)
  - Rating (1-4)

## Circle

- Circle ID - Primary Key. Represented as either an `_id` key in CouchDB.  `ID` table column MySQL database.
- User ID
- Is Default?
- Friends
  - User ID

## Session

The system should suggest the best option based upon my preferences, friends preferences and session history.  If I don't like that option, I can elect to view additional restaurant options.  I want to pick the best option and save it to my session.

- Session ID - Primary Key. Represented as either an `_id` key in CouchDB.  `ID` table column MySQL database.
- Circle ID - Optional. The friends circle related to this session.  Use to populate the session's Friends collection.  
- Friends - A collection of friends associated with this session.  User ID's can be added or removed from this collection.
  - User ID
- Session Date/time
- LunchIt Recommendations - A collections of restaurants recommended by the app.  
  - Restaurant ID
    - Votes - As a friend who is in a circle, I want the ability to open the current LunchIt! session that I am associated with and up-vote or down-vote a LunchIt! recommended restaurant and optionally provide a related comment.
      - User ID - The ID of the friend who voted on a particular restaurant.
      - Vote (+1, -1) - A friend can vote a restaurant up or down.
      - Comment
  - LunchIt Recommended Restaurant Rank (1-5)
  - Selected Restaurant (true) - The restaurant that me and my friends decided to eat.  
  - Is Checked In? (True/False) - Track whether the user confirmed they arrived at restaurant.  When true, enable the user the ability to rate the restaurant, mark or it as a favorite in my preferences, or block the restaurant in my preferences.  See **My Restaurant Preferences**.

## Restaurant Data

- Restaurant ID - Primary Key. Represented as either an `_id` key in CouchDB.  `ID` table column MySQL database.
- OpenTable ID - The restaurant id within the OpenTable API.  See https://opentable.herokuapp.com/.
- Name
- Address
- City
- State
- Area
- Postal Code
- Phone  
- Latitude
- Longitude
- Price Rating (1-4)
- Image URL
- Reservation URL

## Friends Directory Data

- User ID
- Name
- Phone
