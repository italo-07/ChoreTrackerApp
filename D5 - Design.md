
                                        	          Deliverable 5 - Design
                                                      Chore Tracker App
                                                   =========================

<h3>1. Introduction </h3>
The Chore Tracker App is designed to address a common issue plaguing households across the world: the division of labor. Specifically, the Chore Tracker App allows members of a household to assign chores to each other in order to keep organized and get stuff done! The design of the app is based around convenience.The Chore Tracker App is designed as an easy to use tracking tool that takes under 30 seconds to use. We want to create a usable, yet powerful organization tool that prioritizes users' valuable time above all else.

When a user first opens the Chore Tracker App, they are prompted to sign in and create an account with us. This account is stored in our sql database and is used to store information, such as groups and schedules, that are tied to the user. Once logged in, the user can navigate to the add chores section. Here, users can assign themselves chores with a start date and time, end date and time, and a description. Additionally, the user can opt to post the chore in the group they belong to. Groups are added and stored in the database using a seperate form navigated to from the home page. Groups are created by inputting a group name, optional description, and a mutable list of members. The user creating it starts as the first member of the group, and is denoted as an admin. Admins may be added and removed by editing an existing group. Finally, any user can conveniently see their calendar of events by navigating to it from the home page. Here, users can see their chores from any group they are a part of as well as their personal events. Events are displayed as text boxes with a description, and they will programmatically turn from white to an increasing intensity of red if they are not yet completed. If a user marks an event as completed, it will turn green on the calendar. The Chore Tracker App will have all of this functionality implemented and tested to ensure that it conforms to our goal of a <30 second use time. 


<h3>2. Architecture</h3>
This application uses a three layered architecture consisting of the presentation layer, the business layer, and the data access layer. The presentation layer consists of the user interface and the options presented to the user. The business layer contains all of the logic needed to add events, and user's to a group and modify the app settings to the user's preferences. The data access layer consists of the classes needed to access the AWS database and modify the tables within it.

![System Architecture(https://github.com/zachspiel/ChoreTrackerApp/blob/master/Image%20Resources/HighLevelArchitecture.jpg)
