# Template to run and deploy the results from a Cohort Diagnoatics

This repository will provide you the necessary steps to deploy the results of a Cohort Diagnostics.

## To run a Cohort Diagnostics

Follow this template: https://github.com/oxford-pharmacoepi/CohortDiagnosticsTemplate

## To connect shinyapps.io with your account

You will need an account on shinyapps.io to deploy a shinyapp there. 
- There are free accounts: (https://www.shinyapps.io/admin/#/signup)
- The group has an account: ask Dani, Ed or Marti for the details.

Once you have one accout you have to link it with your r session: https://shiny.rstudio.com/articles/shinyapps.html

## To run the local version of the shiny app:
1. Put the resultant 'PreMerged.RData' file in data folder.
2. Open the project in the R session ('CohortDiagnosticsShiny.Rproj')
3. Load all the necessary libraries using renv.
   - renv::activate()
   - renv::restore()
   - y (to accept all the packages that are needed to install, this step can take several minutes)
4. Run the local shiny app
   - shiny::runApp()
5. Youre local shiny app is ready!

## Deploy the shiny app to shinyapps.io

For this step you previously had to connect your R session to shinyapps.io

1. Click the publish icon on the top-right of the local shiny app.
2. It may ask you to update some packages, if it is the case, click yes.
3. Select all the files (by deafult everything is selected) and click: Publish.
4. A new tab (Deploy) next to Console and Terminal will appear. You don't have to do anthing, just wait till the process is finished.
5. The process will be finished when in the Deploy tab shows the following message: 'Application successfully deployed to https://xxxxx.shinyapps.io/xxxxx'
6. Automatically the deployed shinyapp will be opened in your default browser.

