# Template to deploy the results from a Cohort Diagnoatics
This repository will provide you the necessary steps to deploy the results of a Cohort Diagnostics.
## To run a Cohort Diagnostics
Follow this template: https://github.com/oxford-pharmacoepi/CohortDiagnosticsTemplate
## To connect shinyapps.io with your account
You will need an account on shinyapps.io to deploy a shinyapp there. 
- There are free accounts: (https://www.shinyapps.io/admin/#/signup)
- The group has an account: ask Dani, Ed or Marti for the details.

Once you have one accout you have to link it with your r session: https://shiny.rstudio.com/articles/shinyapps.html
## To deploy the shiny app:
1. Put the resultant 'PreMerged.RData' file in data folder.
2. Load all the necessary libraries using renv.
   - renv::activate()
   - renv::restore()
3. Run the local shiny app
   - shiny::app()
4. You can take a look to the local shiny app.

For the next step you previously had to connect your R session to shinyapps.io
5. To deploy this shiny appp to shinyapps.io you have to:
   - Click the publish icon on the top-right of the local shiny app.
   - Select all the files (by deafult everything is selected).
   - Choose an appropiate name and click: deploy.
   -  


