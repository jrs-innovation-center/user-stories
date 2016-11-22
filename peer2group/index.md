[Home](/)  |  [Data](/peer2group/data)

# Peer2Group User Stories

## Overview

A progressive web application (PWA) that enables recreational service industries to drive revenue via a peer-to-peer marketing and sales model. P2P encourages customers to engage other customers by advocating a product or service to friends or associates. A customer is incentivised with discounts when friends and associates sign up for a group recreational activity. The higher a customer is on the _booking pyramid_ the greater the discount percentage.  The discount is multiplied by the number of friends they recruit on the activity.

# Add Activity to Schedule

As an administrator, I need to determine the dates and times that my company will offer an activity to customers.  After adding an activity to the schedule, the activity will appear on the _Activity Calendar_.  

## List Activities By Location

As a customer, I would like to see the various activity locations.  Group all the activities by location.  Once I select a location, I will see a list of activities.  Selecting an activity will route me to a webpage where I can see more activity details.  See **Display Activity Details**.

## List Activities By Duration

As a customer, I would like to see the various activities by duration in hours.  Once I select a duration, I will see a list of activities.  Selecting an activity will route me to a webpage where I can see more activity details.  See **Display Activity Details**.

## Display Activity Details

As a customer, I want to review the details of an activity such as images, description, location, duration, itinerary, inclusions, cost, and availability so that I can make a decision on whether I want to book the activity.  I want to see all the activity details and availability on a single web page. If I decide to book, I need an easy way to begin the process.  See **Book an Activity**.

See [Activity Data](/peer2group/data) and [Activity Schedule Data](/peer2group/data).  

## Display Activity Calendar

As a customer, I need to know the dates and times an activity is available to book.  I need to be able to distinguish between an activity that is fully booked and an activity that is not fully booked and how many spaces are available.

## Book an Activity

As a customer, I want to book an activity by providing the names, ages, and addresses of the people in my group.  As part of the booking, I want to select the name of my friend who recruited me on the activity, so they can receive a discount.  

Confirming my order adds my customer information into the system as well as my booking information.  See [Booking Data](/peer2group/data).  

## SMS Notify Customer of Friend's Booking.

As a customer who has recruited friends, I want to be notified whenever a booking occurs and I have been named as the customer's friend.  As part of the notification, include the following information:

  - Friend's Name
  - Discount Percentage Applied
  - Total Savings
  - Current Discounted Cost

## View My Booking Pyramid

As a customer, I want to see all by P2P activity for a given activity.  I should only be able select an activity that I am associated with.  The display of the booking pyramid should a hierarchical view of all my friends and their friends who have signed up.  I also want to see my discount percentage and my total savings.  

## View a Booking Pyramid

As an admin, I wat to see all the P2P activity for any selected activity.  The display of the booking pyramid should a hierarchical view of all customers who have signed up.  I also want to see my discount percentages and total savings by persons.  I want to see a summary of the total discount given for the entire activity versus full retail cost.
