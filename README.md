# chupiEventCalendar
Easy JS Calendar with event management.  
## How To
Create a ChupiEventCalendar object and provide a container as parameter in the constructor:  
`var calendar=new ChupiEventCalendar(containerDiv)`;
  
Use it!  

##API  

`.setDate(Date date)`  
Change the current date in the calendar.  
  
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
