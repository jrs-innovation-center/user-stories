[Home](/) | [User Stories](/schedulehouse/)

# ScheduleHouse Data

## Property Details

The data elements below represent details for a given property, such as a house. This information is displayed on the Property Details page.

  - Property ID  - Primary Key. Represented as either an `_id` key in CouchDB.  `ID` table column MySQL database.
  - MLS Number - a business/alternate key for the property.
  - Description
  - Pictures
  - Square Footage
  - Number of Bedrooms
  - Number of Bathrooms
  - Type (single family home)
  - Year Built
  - Address
  - Price
  - Active
  - Access details (private)
    - Access Type
    - Access Notes
  - Alarm information (private)
    - Arm Code
    - Disarm Code
    - Passcode
    - Alarm Notes
  - Listing Agent Notes (private)
  - Latitude
  - Longitude

## Showing

The data elements below represent the data elements for a single showing.  This data is used to schedule a showing and obtain feedback from the agent and buyer on the property.  Showing ID is system generated.

  - Showing ID - Primary Key. Represented as either an `_id` key in CouchDB.  `ID` table column MySQL database.
  - Property ID
  - Agent ID
  - Buyer ID
  - Schedule Date
  - Showing Start DateTime
  - Showing End DateTime
  - Status (Buyer Requests Showing, Agent Scheduled)
  - Feedback
    - Buyer Interest Rating
    - Overall Experience Rating
    - Agent Price Opinion Rating
    - Buyer Price Opinion Rating

## Buyer

The Buyer data elements represent a single buyer and any related agents.  Biographical data provided during the signup process. Buyer ID is system generated.

- Buyer ID - Primary Key. Represented as either an `_id` key in CouchDB.  `ID` table column MySQL database.
- First name
- Last name
- Current address
- Cell phone
- Agents - A collection of agents associated with the buyer.
  - Agent ID

## Agent

The Agent data elements represent a single agent in the system.  Data provided during the signup process. Agent ID is system generated.

- Agent ID - Primary Key. Represented as either an `_id` key in CouchDB.  `ID` table column MySQL database.
- First name
- Last name
- Current address
- Cell phone
