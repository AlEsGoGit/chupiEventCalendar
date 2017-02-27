# chupiEventCalendar
Easy JS Calendar with event management.  
## How To
Create a ChupiEventCalendar object and provide a container as parameter in the constructor:  
`var calendar=new ChupiEventCalendar(containerDiv);`  
Also, you can set an object "options" as second parameter.
  
Use it!  

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
  
`nextClick(Function callback)`  
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
