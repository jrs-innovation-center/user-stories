[Home](/) | [User Stories](/my5/)

# My 5 Data

## Lists

- List ID - Primary Key. Represented as either an `_id` key in CouchDB or `ID` table column in a MySQL database. Uniquely identifies a list amongst all other lists.
- List Category (Ex: Music, Movies, Books, etc. )
- List Name (Ex: Top 5 Beatles Albums)
- List Description (Ex: The definitive list of the best Beatles Albums.  Let the debate begin!)
- List Creator User ID (The user id of the person who created the list.)

## List Items

(Items in the list, such as Album Names)

- List Item ID
- List ID - The list to which the list items belong.
- List Item Name (Ex: Magical Mystery Tour)
- List Item Creator Rank (My rating of the item in the list. Ex:  My top rated Beatles album, such as Magical Mystery Tour, would have a List Item Creator Rating = 1)

## List Item Vote

- List Item Vote ID - Primary Key. Represented as either an `_id` key in CouchDB or `ID` table column MySQL database.
- List Item ID
- User ID - The user id of the person who up or down voted the item on the list.
- Vote (Ex: An up or down vote for the given List Item.  Value is either a +1 or -1).
