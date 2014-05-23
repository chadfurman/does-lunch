## General Requirements

Employees will be able to visit the app and create a lunch run. 

When a lunch run is created, it will send notifications to the entire group of users. Email and/or mac growl notifications.

It should be 2 pages. One for creators, and one for everyone else ordering.

App Run and Order data will be automatically cleared every day. It can also be manually cleared.

A User (that has placed an order in the current day's run) must be chosen randomly 


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
