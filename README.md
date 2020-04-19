# CoronavirusTweet
Coronavirus tweet analysis

Here's the demo app: https://hannahwang.shinyapps.io/CoronavirusTweet/

1. For now, haven't really adjusted the user interface..so it might not be that straightforward
(1) The "Date input" and "flock of interest" controls the word frequency sessions, you can click through! Word frequency by 
by flock can contain multiple flocks. The maximum is you can choose all 6 of them.
(2) The "Topic cluster","choose one flock", and "Date Input" widgets can all control the 2nd tab-tweet wall. It will filter
the topic cluster for a specified flock on a specific date, please feel fre  to try it out.

2. For coding...I also depend largely on google lolol, here's a gallery that I refer to a lot, they have many templates and 
coding example: https://rmarkdown.rstudio.com/flexdashboard/examples.html. This one is useful too: https://www.robbyshaver.com/rmarkdown7/gallery.html. 
I usually open a data processing file first to see if the code can work in static. After that, I adjust the code to the 
shinyversion. For this project, I put most user input widgets in the "Sidebar" chunck. Also, the datasets that will change 
according to user input, is often wrapped in the reactive() function, and I also put those in the "Sidebar" chunck, just for 
convenience. 
