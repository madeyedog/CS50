# CS50 Project: Personal Relationship Manager
## Problem: 
As time goes on, I find it harder to keep track of the people in my personal and professional life. This includes missing birthdays, forgetting what they were last up to, how old their kids are, if they have moved, etc. I think a simple solution to keep track of friends and family and key information about them would be very handy, and doing so in a way that is more of a relationship manager than social media would be helpful.

### Requirements:
- Users should be able to create an account
- Users should be able to add a contact
- Users should be able to add an interaction with a contact
- Data model must account for first and last name, phone number, email, interactions with the people, as well as being able to identify 'life events' - major events that should be marked with a date and reminders shared where appropriate (e.g., birthdays)
- There should be at least two views: (1)An overall contact list that provides the name, contact info, and last interaction with the person
        (2) A list of the interactions with an individual
- There should be a feature that suggests reaching to a friend that you have not been in touch with for over a year
### Design Decisions:
- A contact should exist befor an event or interaction can be added for that contact
- The index view should present the reminders
- For checking how long since an interaction, it is a better use of resources to pull the latest interaction for each contact and then check time frame, then pull contact info. This is better than pulling all records then checking timeframe

### Ideas for future build out:
 - Search and select for contacts so the user doesnt have to enter the full name each time
 - Batch entry of interactions, events, contacts
 - Hooks into Facebook, gmail, etc to pull in available info so the use doesnt have to enter it
