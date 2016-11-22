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

- Session ID - Primary Key. Represented as either an `_id` key in CouchDB.  `ID` table column MySQL database.
- Circle ID
- Friends
  - Friend ID
- Session Date/time
- LunchIt Recommendations
  - Restaurant ID
    - Friend vote
      - Friend ID
      - Vote (+1, -1)
      - Comment
  - LunchIt Recommended Restaurant Rank (1-5)
  - Selected Restaurant (true)
  - Is Checked In? (True/False)

## Restaurant Data

- Restaurant ID - Primary Key. Represented as either an `_id` key in CouchDB.  `ID` table column MySQL database.
- OpenTable ID
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
