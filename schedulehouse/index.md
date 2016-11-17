[Home](/)  |  [Data](/schedulehouse/data)

# ScheduleHouse User Stories

> As a _type of user_, I want _some goal_ so that _some reason_.

## Overview

Showing scheduling and management for real-estate agents and home buyers.

## Search Properties

0. As a user, I want to search my MLS listings in the following ways:

  - MLS #
  - Street Address
  - Square Footage
  - Number of Bedrooms
  - Number of Bathrooms

0. Once a single property is selected, display the property based on the current user's role. See **Display Property Details (By Agent)** and Display Property Details (By Buyer).  

## Sign Up

0. As a potential user of the system, I need a way to sign up and provide my personal details.  I want the option to sign up as one of the following roles:

  - Agent
  - Buyer

0. As a potential home buyer, I wish to indicate which agents I am currently working.  

## Sign In

0. As a user, I need a way to sign into the system so that I can access my relevant information.  

## Distinguish Roles

0. As an administrator of the system, I need to designate users into one of the following roles. Only an administrator can place a user in a role.

  - Agent
  - Buyer
  - Administrator.

0. As a potential home buyer, I need to:

  - Access my biographical information
  - Search properties
  - View property details
  - Request showings
  - Rate houses I visit during a showing.

0. As a realtor, I need to:

  - Access my biographical information
  - Search properties
  - View property details
  - Schedule showings
  - Rate houses I visit during a showing

##  Display Property Details (By Agent)

0. As a real estate agent, I want to view the following public _and private_.

See [Property Details Data Elements](data#property-details).

##  Display Property Details (By Buyer)

0. As a potential home buyer, I want to view the following public details for a specific property.

See [Property Details Data Elements](data#property-details).

## Schedule Showing by Agent

0. As a real estate agent, I want to schedule a showing of a property from the **Property Details Page**. (See **Display Property Details By Agent**) Scheduling involves a real estate agent selecting a buyer, selecting a schedule date, and selecting available start and end times for the property.

See [Showing Data Elements](data#showing).

## Request Showing by Buyer

0. As a potential home buyer, I want to request a showing of a property from the property details page. (See **Display Property Details By Seller**)  Requesting involves selecting a date, reviewing available times for the property, and selecting an available start and end time.

See [Showing Data Elements](data#showing).

## Map Property

0. As a user, while I'm viewing the details of a specific property, I want to see where a property is located on a map.  

## Search Buyers By Last Name

0. As a real estate agent, I want the ability to search though my buyers by Last name.

0. Once selected, **Display Buyer**.  

## Search Buyers from A to Z

0. As a real estate agent, I want the ability to browse though my buyers from A to Z.

0. Once selected, **Display Buyer**.

## Display Buyer

0. As a real estate agent, I need a **Buyer Details Page** to view the details on an individual buyers .

See [Buyer Elements](data#buyer).

## Display Calendar for an Agent's Showings

0. As a realtor, I want to see a calendar that displays my related showings for _all_ the properties for _all_ my buyers.  Each showing on the calendar should display:  

  - Showing Start Time
  - Showing End Time
  - Property Street Address
  - Buyer Last Name

See [Showing Data Elements](data#showing).

0. Selecting a showing on the calendar provides the following options:

- Navigating to the **Buyer Details Page**
- Navigating to the **Property Details Page**
- Filter Calendar for Buyer's Showings
- Filter Calendar for Property's Showings
- Navigate to the Realtor's **Daily Showing Schedule Page**.
- Navigate to the Buyer's **Daily Showing Schedule Page**.
- Navigate to the Property's **Daily Showing Schedule Page**.

## Filter Calendar for Buyer's Showings

0. As a realtor, I want to see a specific buyer's schedule.  I want to see a calendar that displays _all_ the showings for a _specific_ buyer.  Each showing on the calendar should display:  

  - Showing Start Time
  - Showing End Time
  - Property Street Address
  - Buyer Last Name

See [Showing Data Elements](data#showing).

0. Selecting a showing on the calendar provides the following options:

  - Navigate to the **Buyer Details Page**
  - Navigate to the **Property Details Page**
  - Filter Calendar for Buyer's Showings
  - Filter Calendar for Property's Showings
  - Navigate to the Realtor's **Daily Showing Schedule Page**.
  - Navigate to the Buyer's **Daily Showing Schedule Page**.
  - Navigate to the Property's **Daily Showing Schedule Page**.

## Filter Calendar for Property's Showings

0. As a realtor, I want to see when a specific property is available for showing.  I want to see a calendar that displays all showings for a _specific_ property across all realtors.  Each showing on the calendar should display:  

  - Showing Start Time
  - Showing End Time
  - Property Street Address
  - Buyer Last Name

See [Showing Data Elements](data#showing).

0. Selecting a showing on the calendar provides the following options:

  - Navigate to the **Buyer Details Page**.
  - Navigate to the **Property Details Page**.
  - Filter Calendar for Buyer's Showings.
  - Filter Calendar for Property's Showings.
  - Navigate to the Realtor's **Daily Showing Schedule Page**.
  - Navigate to the Buyer's **Daily Showing Schedule Page**.
  - Navigate to the Property's **Daily Showing Schedule Page**.

## Display Realtor Showing Schedule for a Specific Day (Daily Showing Schedule Page)

0.  As a realtor, I want to see my showing schedule for a specific day on a **Daily Showing Schedule Page**.

0. Selecting an item on the Showing Schedule provides the user with the following options:

  - Route the app to the **Buyer Details Page**.
  - Route the app to the **Property Details Page**.
  - Route the app to the Buyer's **Daily Showing Schedule Page**.
  - Route the app to the Property's **Daily Showing Schedule Page**.

## Display Buyer Showing Schedule for a Specific Day (Daily Showing Schedule Page)

0. As a buyer, I want to see my showing schedule for a specific day on a **Daily Showing Schedule Page**.

0. Selecting an item on the Showing Schedule provides the user with the following options:

  - Route the app to the **Buyer Details Page**.
  - Route the app to the **Property Details Page**.

## Display Property Showing Schedule for a Specific Day (Daily Showing Schedule Page)

0.  As a realtor, I want to see the showing schedule for a specific property for a specific day on a **Daily Showing Schedule Page**.

0. Selecting an item on the Showing Schedule provides the user with the following options:

  - Route the app to the **Buyer Details Page**.
  - Route the app to the **Property Details Page**.
  - Route the app to the Buyer's **Daily Showing Schedule Page**.
  - Route the app to the Realtor's **Daily Showing Schedule Page**.

## Map Property (Property Details Page)

0. As a user of the system, when I am viewing property details on the **Property Details Page**, I desire the need to see where a specific property is located on a map.  

## Map Properties (Map Properties Page)

0. As a user of the system, when I am looking at my showing schedule, I desire the need to see where a specific set of properties are located on a map.  

## Reveal Mapped Property Details (Map Properties Page)

0. Selecting a specific mapped property on the map reveals the following property details:

  - Address
  - Price
  - Photo
  - Link to **Property Details Page**.
  - Navigate my vehicle to the property address.

## Rate houses

0. As a realtor or buyer, I need the ability rate housing during or after the designated showing start time.  I would prefer to provide my ratings on the **Property Details Page**.  

0. Do not allow me to provide a rating before the designated showing start time.

0. As a buyer, I need the ability to provide the following feedback on a property:

  - Buyer Interest Rating
  - Overall Experience Rating
  - Buyer Price Opinion Rating

0. As an agent, I need the ability to provide the following feedback on a property:

  - Agent Price Opinion Rating

## SMS - Notify Agent of Buyer Interest in Property

As a potential home buyer, I wish to let my agent

## SMS - Notify Buyer of Schedule Change

## SMS - Buyer Sends Link to Property (Property Details Page) to Agent

## SMS - Agent Sends Link to Property (Property Details Page) to Buyer

## Adjust Agent Showing Schedule

0. As a realtor, I need to adjust my showing schedule for a specific day on a **Daily Showing Schedule Page**. I'd like to reorder my showings by dragging items above or below one another.  

0. Once saved, **SMS - Notify Buyer of Schedule Change**.
