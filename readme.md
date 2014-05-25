# Fuzz Lunch #
A simple app for food runs

## General Requirements
Simple, minimal, and intuitive.  Supports IE9+ and all mobile devices.

Any Lunch Run Creator will be able to visit the app and create a lunch run. 

When a lunch run is created, it will send notifications to the entire group of Eaters.  Email and/or mac growl notifications. ** Maybe just give a link.  See 'how a lunch is created' below**

It should be 2 pages. One for creators, and one for everyone else ordering.

App Run and Order data will be automatically cleared every day. It can also be manually cleared.  ** No need to save data, though maybe there could be a restauraunt promotion system based on geolocation data **

A User (that has placed an order in the current day's run) should be chosen randomly as the person to pickup the food

## How is a lunch created
1) Creator comes to site, sees main page which displays "create lunch run" form -- just the Restauraunt Link is needed
3) Creator is given two links after creating the run: order form and review order page
3a) Creator emails the order form to Eaters
4) Eaters click on link, see "order food" page -- Restauraunt link, Name, Food Order, Volunteer to pick-up
6) Eaters order appears on the review order page after eaters enter their data
8) Order is ready to be placed when all users enter their data

## Data to be modeled (collections):

Restaurant
  - _id (name)
  - address_link (google map link)
  - menu_link
  - delivers (boolean)
  - popularity (based on User input)

User
  - _id (name)
  - password (LDAP?)
  - email

Run
  - _id
  - restaurant
  - creator_id
  - user_id (array)
  - order_id (array)

Order
  - _id
  - volunteer (to pick up the food)


## Required Features


## Page-specific Details
