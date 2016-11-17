[Home](/)  |  [Data](/goodtimes/data)

# Goodtimes User Stories


## Overview
A progressive web application (PWA) that enables recreational service industries to drive revenue via a peer-to-peer marketing and sales model. P2P encourages customers to engage other customers by advocating a product or service to friends or associates. A customer is incentivised with discounts when friends and associates sign up for a group recreational activity. The higher a customer is on the "friend pyramid" the greater the discount percentage.  The discount is multiplied by the number of friends they recruit on the activity.

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

## Display Activity Details

## Book Activity





# Goodtimes Data

## Booking Data

Track the booking information for a customer for an activity on a specific day and time. Indicates whether the customer is the "leader" (Is P2P Customer Leader?). Indicates if the customer was recruited by a parent customer (P2P Parent Customer ID).  

- Activity ID
- Booking Start Date and Time
- Customer ID
- Is P2P Customer Leader? (True/False)
- P2P Parent Customer ID
- Booking Date
- Booking Time
- Price
  - Price Type (Adult/Child/Senior)
  - Price Amount 

## Activity Data

- Activity ID
- Activity Name
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
- Address
