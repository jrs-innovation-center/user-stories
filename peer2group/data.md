[Home](/) | [User Stories](/peer2group/)

# Peer2Group Data

## Booking Data

Each booking item represents a single customer's booking or reservation on a specific day and time for a specific group activity such as rock climbing or paddle boarding.
As part of a booking the customer can indicate whether they were referred by a friend.  

A _Booking Pyramid_ is formed by creating a hierarchy of the booking data.  The **P2P Customers Friend ID** field/column/key/property designates whether the customer was referred by a friend. If so this field holds the friend's customer ID.    

** Booking Pyramid Example **

```
Activity: SUP Eco Tour (Costs: Adult - $120.00USD, Child - $120.00USD, Senior - $80.00USD)
 \__ Mary (Leader) (Discount Pct: 10%, Peer Count: 7, Total Discount: 70%)  
      \___ Joe (Friend) (Discount Pct: 0%, Peer Count: 0, Total Discount: 0%)  
      \___ Jeff (Friend) (Discount Pct: 0%, Peer Count: 0, Total Discount: 0%)  
      \___ Jerry (Friend) (Discount Pct: 5%, Peer Count: 4, Total Discount: 20%)  
            \___ Sam (Friend) (Discount Pct: 0%, Peer Count: 0, Total Discount: 0%)  
            \___ Steve (Friend) (Discount Pct: 0%, Peer Count: 0, Total Discount: 0%)  
            \___ Sara (Friend) (Discount Pct: 0%, Peer Count: 0, Total Discount: 0%)  
            \___ Sumir (Friend) (Discount Pct: 0%, Peer Count: 0, Total Discount: 0%)  
```
- Booking Item ID - Primary Key. Represented as either an `_id` key in CouchDB.  `ID` table column MySQL database.
- Activity ID
- Schedule ID
- Booking DateTime - The date and time the customer booked the activity.
- Customer ID
- Is P2P Customer Leader? (True/False) - customer is the "leader" and eligible for the top discount.
- P2P Customers Friend ID - Indicates the customer was recruited by a friend (P2P Customers Friend ID).
- Price
  - Price Type (Adult/Child/Senior)
  - Price Amount

## Activity Schedule Data

Tracks the date, time, and availability of when the activity is available.

- Schedule ID
- Activity ID
- Activity Start DateTime
- Openings Available? (True/False)

## Activity Data

- Activity ID
- Activity Name
- Duration in Hours
- Location Name
  - Mapping waypoint
    - Latitude
    - Longitude
- Prices
  - Price Type (Adult/Child/Senior)
  - Price Amount  
- Booking Minimum
- Booking Maximum
- Discount Structure
  - Leader
    - Discount Pct
    - Max Discount Pct
  - Friend  
    - Discount Pct
    - Max Discount Pct
- Images
- Itinerary Steps
  - Itinerary Step Number/Order
  - Itinerary Description
  - Mapping waypoint
    - Latitude
    - Longitude
- Pickup
  - Description
  - Mapping waypoint
    - Latitude
    - Longitude
- Drop Off
  - Description
  - Mapping waypoint
    - Latitude
    - Longitude
- Things to bring
- Inclusions
- Exclusions
- Cancellation Policy


### Activity Data Example

<table width="100%">
  <col style="width:15%">
  <col style="width:45%">
  <col style="width:40%">
  <thead>
  <tr>
    <th>Key/Column</th>
    <th>Example</th>
    <th>Description/Notes</th>
  </tr>
  </thead>
  <tr>
    <td>Activity ID</td>
    <td>Annaberg</td>
    <td></td>
  </tr>
  <tr>
    <td>Activity Name</td>
    <td>Hike and Snorkel</td>
    <td></td>
  </tr>
  <tr>
    <td>Prices</td>
    <td>Adult ($120.00 USD)<br>
    Child ($60.00 USD)<br>
    Senior ($80.00 USD)
    </td>
    <td></td>
  </tr>
  <tr>
    <td>Minimum Required To Book</td>
    <td>2</td>
    <td></td>
  </tr>
  <tr>
    <td>Maximum Allowed</td>
    <td>10</td>
    <td></td>
  </tr>
  <tr>
    <td>Discount Structure</td>
    <td>Leader Discount Pct: 10%, Max Discount Pct: 80%<br>
    Friend Discount: 5%, Max Discount Pct: 60%<br></td>

    <td>The Hike and Snorkel group activity incentivises the leader with a 10% "Leader" discount for each person they recruit, with a maximum discount percentage of 80% off the retail price.  Any friends of the leader who recruit additional friends receive a 5% discount for each person they recruit, with a maximum discount percentage of 60% off the retail price.</td>
  </tr>
  <tr>
    <td>Images</td>
    <td></td>
    <td>A collection of image file names.</td>
  </tr>
  <tr>
    <td>Itinerary</td>
    <td>
    -  Meet at The VI National Park's Visitor Center in Cruz Bay, St John, and learn about the Park before boarding your taxi to Annaberg Plantation.<br>
    - Explore the ruins of the Annaberg Plantation and learn about the history of this preserved site.<br>
    - Hike to Waterlemon Cay through a portion of the National Park of St. John.<br>
- Safely Snorkel with your professional guide from shore to around Waterlemon Cay and explore the sandy spit beach on Sandy Cay and learn about the sea birds and marine life and among St John's Premier Snorkel Site.<br>
- Hike back to Annaberg Plantation where a taxi will return you to The Visitor Center in Cruz Bay.</td>
    <td>A detailed plan for a journey, especially a list of places to visit; plan of travel.</td>
  </tr>
  <tr>
    <td>Map</td>
    <td>- </td>
    <td>A collection of latitude and longitude map waypoints.</td>
  </tr>
</table>

## Customer Bio Data

- Name
- Birthdate
- Address
