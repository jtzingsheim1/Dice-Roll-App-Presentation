Pitch for Dice Roll! App
========================================================
author: Justin Z
date: June 12, 2019
autosize: TRUE

Navigate using arrow keys or clicking arrow buttons in the lower right corner.


Overview
========================================================

This presentation is for the week 4 peer-graded project in the Developing Data
Products course from Johns Hopkins University within the Data Science
Specialization on Coursera. The instructions say to create an application using
`shiny` and then create a presentation pitching the app.

To meet the objective an application was created which is a game where the user
can place wagers on the outcome of a roll of two dice. The `shiny` application
and this presentation were created in Rstudio.
 - The repo for the app is [here][1].
 - The app is hosted on shinyapps.io [here][2] (accessible as monthly active
 hours allow)

[1]: https://github.com/jtzingsheim1/Dice-Roll-Application "GitHub repo for app"
[2]: https://jtzingsheim.shinyapps.io/Dice_Roll_Game/  "shinyapps.io"


User Interface (Image Only)
========================================================

![UI Screenshot](UI_Screenshot.png)


Server Logic
========================================================

A key feature of the server code is rolling the dice. A modified version of the
actual code is shown and run below. Just like in the actual application, the
seed is intentionally not set.


```r
# Roll the dice and display images
dice <- sample(1:6, 2)
filenames <- paste0("die", dice, ".png")
filepaths <- file.path("die_images", filenames)
knitr::include_graphics(filepaths)
```

<img src="die_images/die5.png" title="plot of chunk server1" alt="plot of chunk server1" width="10%" /><img src="die_images/die2.png" title="plot of chunk server1" alt="plot of chunk server1" width="10%" />


Sales Pitch
========================================================

This is a good app because:
 - It is fun to play
 - It allows users to have a gambling like experience in a safe environment
 - Users can apply their statistics knowledge to exploit the payouts and win big
 - It is a creative solution to the project requirements
 
Thanks for your time, I hope you enjoyed using the app.

