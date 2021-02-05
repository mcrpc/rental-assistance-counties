# Rental Assistance Need in McLean County, Illinois

The analysis presented here is adapted from the analysis presented by NYU Furman Center in this blog post:

[Rental Assistance Need in Five of New York’s Mid-Sized Cities](https://furmancenter.org/thestoop/entry/rental-assistance-need-in-five-of-new-yorks-mid-sized-cities)

## Notes for future users:

### Running the analysis

If you are running this code for the first time, ensure you have the latest version of [R](https://www.r-project.org/) and [RStudio](https://rstudio.com/) installed first. Then, you will want to open the `rental-assistance-mclean` R Project file in RStudio.

This analysis uses R Markdown to run R code contained within code chunks and separate R scripts and then "knits" the tables of data into HTML reports. For a bit more background on how this works, consult [this quick overview page](https://rmarkdown.rstudio.com/authoring_quick_tour.html) from the RStudio development team.

In order to run the code you will need to 'knit' the `prep-data` and then the `analysis` R Markdown files. You may need to run the second code chunk in the `analysis` file which installs necessary packages in order to have access to this function or for it to work properly.

Whenever you make updates to the analysis, make sure to push changes to the [GitHub repository](https://github.com/mcrpc/rental-assistance-mclean). This will populate [a website](https://mcrpc.github.io/rental-assistance-mclean/) where the HTML reports generated by the analysis code are accessible in all of their glory. The more diligently you update the GitHub repo, the easier your life will be if you need to revert back to earlier versions or collaborate on this project. For more information on using GitHub, consult the readme file in the RPC GIS drive or check out [this quick guide](https://happygitwithr.com/rstudio-git-github.html).

### Updating the input data

Search for lines of code with the keyword #CHANGETHIS when updating with new BLS or IPUMS data. Most of these lines can be found in the files renter_unemp_adj.R, bls-emp-il.R, and prep-data.Rmd, but be sure to scan the rest of the analysis code for references to dates that may need to be updated, particularly in the blocks of descriptive text.

### Maintaining the analysis code

The code behind this analysis *should* work just fine for the foreseeable future. However, R packages change and functions become deprecated over time, so keep an eye out for warning and error messages to that effect. Package authors (particularly in the `tidyverse` group of packages) are *usually* quite good at letting you know when things will become deprecated and giving you suggested changes well in advance, but not always. If something breaks and you cannot figure out why, take advantage of RStudio's debug tools and try to isolate the problematic lines of code. When all else fails, search in places like [stackoverflow](https://stackoverflow.com/questions/tagged/r) and you will likely find other users working through similar problems.

### Modifying the analysis

Making changes to the format and methods of this analysis will require a significant background in R. Whether you are a beginner who is interested in getting started with R or an R user who is unfamiliar with the `tidyverse`, the free guide [R for Data Science](https://r4ds.had.co.nz/) is an excellent place to start. When in doubt, always start small and constantly re-run the code to check your outputs.
Add a sentence here.
--- 

[Details on data preparation](https://mcrpc.github.io/rental-assistance-mclean/docs/prep-data.html) 

[Details on analysis and results](https://mcrpc.github.io/rental-assistance-mclean/docs/analysis_moe-no_rep-100.html)
