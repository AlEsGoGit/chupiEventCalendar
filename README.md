# chupiEventCalendar
Easy JS Calendar with event management.  
## How To
Dowload the .js and the .css and import them.  
Create a ChupiEventCalendar object and provide a container as parameter in the constructor:  
`var calendar=new ChupiEventCalendar(containerDiv);`  
Also, you can set an object "options" as second parameter.
  
Use it!  

Customize the css if you want to.
##API  

`.setDate(Date date)`  
Change the current date in the calendar.

`.setOptions(Object options)`  
Change the current options.  
See below for options details.
  
`.loadEvents(Array events)`  
Load the events wich have to be marked in the calendar.

`.removeEvents()`  
Remove the current events loaded.  
  
`.refresh()`  
Repaint the calendar. Needed after changing events, date...  
  
`.loadEventsPanel(Array events)`  
Provide the events you want to be displayed below the calendar.  
  
`.showEventsPanel()`  
Show the panel below the calendar.  
  
`hideEventsPanel()`  
Hide the panel below the calendar.

`previousClick(Function callback)`  
You can provide a function you want to be "triggered" when the previous button is clicked.  
  
`nextClick(Function callback)`  
You can provide a function you want to be "triggered" when the next button is clicked.  
  
`dayClick(Function callback)`  
You can provide a function you want to be "triggered" when a day is clicked.  


##Options  
Options are set as a default java script object.  
These are the available options:  
* `lang: "en"|"es"`  
language for days and months.  
"en" default.  
* `firstDay`  
number of the first day of the week.  
"1" for Sunday.  
1 default.  
  
Adding more options...

##Events  
The calendar needs an array of Events objects to work properly.  
The object Event has these properties:  
* day  
* month  
* year  
* title  
* content


##Example  
To prevent you from loading a lot of events at the same time, you have available the previous/next/dayClick() methods, that allow you to set a custom callback for their event listeners.  
You can set an ajax request wich will be launched everytime you click one day-cell, so you can load|show only the events for that day. 
Also, you can do the same every time you change the date, loading only the events for the previous/next month.  
Then you can use the loadEvents() and loadEventsPanel() to mark those events in the calendar or display them inside the panel below the calendar.
