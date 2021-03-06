Project Description:
====================

The department of Transportation and Facilities Management wants to create a centralized system that will create and manage the logs created by shuttle-bus drivers on campus. These drivers currently write the data onto paper and then digitize this information on a computer at a later time. This new system should also represent the data to a supervisor in a useful way.

Use Cases:
==========

1.  As a shuttle bus driver, I will enter and submit any stop information on the tablet.

2.  The system should update in the background when internet connectivity has been established/reestablished.

3.  As a supervisor, I should be able to add information to the database regarding new stops and new busses.

4.  As a supervisor, I will edit or modify entries in the database to fix mistakes.

5.  As a supervisor, I will be able to view the real-time information on my desktop.

6.  As a supervisor, I will be able to export the real-time information to be used in other software.

7.  The system shall display stop information by the hour.

8.  As a supervisor, I will be able to filter and display stop information.

9.  The system shall be viewable by more than one user at a single time.

User Classes and Characteristics:![](https://lh4.googleusercontent.com/Be-L2oiTKQODsG9pjnI-puGkSwaeW0ohJibFrJqN5Gp3tqvoI9VrYk-T-arEiN5aS1FCNJmcvaonpl6Qn_x0OnKlsaBldwSZhmItCk5K7aksK3q3uMK_q25H1KWiWxZ4WnvbzNGX)
================================================================================================================================================================================================================

Driver: The driver is the primary user of the "mobile system" of the application. They will use the application when they are stopped at their stops. They will use the application to record how many people are using Ball State's buses.

Standard User: The standard user will use the "desktop system". It will be used to sort the information that is gathered by the drivers into a useful form. The standard user will sort the information into the form that they want, then they will be able to use the application to export the information into a file format that can be imported into microsoft Excel.

Admin: The admin will be able to sign into the application with their credentials to access features of the desktop system that is not available to the standard user. The admin will be able to update and correct information from the drivers. The admin will also be able to add/edit/delete buses/loops/stops.

Technical Constraints:
======================

-The buses may not have an internet connection at all times, so the mobile system must be able to work without an internet connection.

-The mobile system needs to be able to save the information when it doesn't have an internet connection and then push it when it has a connection.

-The Desktop system needs to be able to work with the new information by refreshing in the background.

Requirements
============

Functional and Non-Functional:
---------------

Driver Requirements | Currently Exsisting 
------------ | -------------
Set the amount of people getting on the bus | Increment and deincerment buttons to count passengers
"Sign on" at the start of their shift | Login screen for driver application
Select the stop | Drop down bar to select stop and automatically switches to the next stop
Be alerted if the the information was pushed or not | Error message notifying if data was not synced
see a log for the day | Entries page on Desktop listing all data for the day
see if their information was pushed | Sync button on configurations page showing if data still needs to be synced efore logging out
say if anyone was left behind | Increment and deincrement buttons to count passengers left behind at stop
must work with sporatic internet connection | Driver application holds data until reconnected to internet and must be synced before logging out of application. Mobile hotspots and cellular ipads are being placed into the busses to compensate for internet loss
easy to use | Minimal interactions on driver application so driver isn't confused on how it is used
not distracting | Simple 2-page application that limits driver usage and creates less distraction
must be fast | Syncs data to desktop after 30 seconds in-between stops


------------------------------------

Desktop Requirements | Currently Exsisting 
------------ | -------------
view the information from the drivers | Entries page on desktop showing data from drivers
view the information as it is being updated | Entries page on desktop showing data from drivers as it is being entered in
filter information | Entries page can filter data by the date and the loop
export information | Reports page on destop allowing admin to export an CSV file
add/edit/delete buses/loops/stops | Add/Edit/Delete icons added to Stops/Loops/Users pages to change information on desktop
easy to use | Simple Desktop User Interface allowing admins to easily navigate through different pages


Assumptions:
============

-   We assume that they'll need a feature that will indicate whether students were left behind or not.

-   There are a few formats that we could export to but we still haven't talked about how exactly they'll use the exported data.
