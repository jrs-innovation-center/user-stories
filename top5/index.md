[Home](/)  |  [Data](/top5/data)

# Top 5 User Stories

> As a _type of user_, I want _some goal_ so that _some reason_.

## Overview

A website that allows users to post their top 5 favorite things and allows friends the ability to provide their opinions via votes and comments.  Associated with the top 5 lists, a blog provides insights into how the top 5 was formed.  Blog posts can have comments which can be voted upon.  Visitors can view lists and comments but can not vote or add a comment.  Users can create lists, vote and comment.

## View Categories

As a user (visitor or user) I want to browse the lists by their list category such as:

- Music
- Movies
- Books
- Top Relationship fails

Once I select a category, I am directed to the **Display Lists** page where I see a list of lists.  How meta!

## Display Lists

As a user, I want to view a list of all the lists for a specific category.  Each item in the list should display the following:

- List Name (Ex: Top 5 Beatles Albums)
- List Description (Ex: The definitive list of the best Beatles Albums.  Let the debate begin!)
- List Rank

# Top 5 Data

## Lists

- List ID - Primary Key. Represented as either an `_id` key in CouchDB.  `ID` table column MySQL database. Uniquely identifies a list amongst all other lists.
- List Category (Ex: Music, Movies, Books, etc. )
- List Name (Ex: Top 5 Beatles Albums)
- List Description (Ex: The definitive list of the best Beatles Albums.  Let the debate begin!)
- List Creator User ID (The user id of the person who created the list.)
- List Items (Items in the list, such as Album Names)
  - List Item ID
  - List Item Creator Rating (My rating of the item in the list. Ex:  My top rated Beatles album, such as Magical Mystery Tour, would have a List Item Creator Rating = 1)
  - List Item Name (Ex: Magical Mystery Tour)

## List Item Vote
  - List Item Vote ID - Primary Key. Represented as either an `_id` key in CouchDB.  `ID` table column MySQL database.
  - List Item ID
  - User Rating (Ex: A count of all the up or down votes by other users.  Ex:  A value of '2' represents that other users think the Magical Mystery Tour is the 2nd best album in the list. IF a user up-votes this album, the user rating would increase from 2 to 3. )
