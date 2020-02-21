## Ticket store
An application is developed to allow selling tickets online.
A client must be able to see list of all events, select an event and see what is the ticket cost, how many tickets are left.

### Entities
- customers (respective buyers of tickets)
- event_tickets (bought tickets for events)
- events
- venues
- event_artists
- artists

### Requirements
- customer can register in the system providing (name, surname, email, birthday) 
- customers can update their info, excluding email
- customers can delete their account
- customer can purchase a ticket to a specific event
- customer can view event info
- administrator can perform CRUD operations on Venues 
- administrator can perform CRUD operations on Events
- administrator can perform CRUD operations on Artists
- single customer is not allowed to purchase more then 10 tickets
- customer is not allowed to purchase tickets after the end of ticket sales
- customer is not allowed to purchase tickets before the start of ticket sales
- customer is not allowed to purchase tickets when there are not tickets left
 
--- 
## Fitness equipment store
An application is developed to help keeping track of equipment items in the store and sell them online.
A client must be able to list all equipment, view specific item details, buy an item online.

### Entities
- brands
- articles
- stock
- customers
- orders

### Requirements
- Administrator can perform CRUD operations on brands
- Administrator can perform CRUD operations on articles
- Administrator can perform CRUD operations on stock
- customers can view stock items that are not sold already
- customer can register in the system providing (name, surname, email, birthday) 
- customers can update their info, excluding email
- customers can delete their account
- customers can create an order with multiple stock items
- customers can update an order if it was not already approved or shipped by administrator
- administrator can mark an order as shipped
- administrator can mark an order as approved
- customers can delete their order if it was not shipped already
- customers are not allowed to add stock items that are already in another order to their order
- administrator is not allowed to delete or update stock item after it was added to order


---
## Car accident management
An application is developed to keep track of car accidents in a city, to analyze most dangerous places.
A user must be able to see what accidents have happened, involved parties, location of the accident.
 
### Entities
- users
- cars
- locations
- accidents
- accident_cars
- accident_users

### Requirements
- user can create an account (name, surname, email)
- user can update account info, excluding email
- user can NOT delete his account if there are accidents registered for that user
- user can enter location information where accident has happened (city, street, house nr.)
- user can enter cars that where involved in accident
- user can enter additional users involved in accident (witnesses, victims)
- car driver involved in accident can approve submission of accident
- an accident is considered as submitted when all car drivers have approved submission of accident
- user can delete cars involved in accident if the accident is not submitted
- user can delete additional users involved in accident if the accident is not submitted
- administrator can view list of all accidents


---
## Team Scheduler
An application is developed to help people organize their day/week.
A user must be able to create an event(like a meeting or a call) for a group of users, see all events on a specific date period(day, week, month).


### Entities
- users
- user_teams
- teams
- events
- event_users
- event_teams

### Requirements
- user can create an account (name, surname, email)
- user can update account info, excluding email
- user can delete his account
- user can select one or more teams that he is part of
- user can create an event for one or multiple teams, specifying dates, type of event(meeting, conference call)
- user who created the event can delete or update it 24hrs before the start of the event
- user can join an event if he is assigned to a team that is assigned to this specific event
- user can decline an invitation for specific event
- users can view events that are pending in specified date interval

