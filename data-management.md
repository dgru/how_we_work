# Marine Predator Group Data Management Plan

The Marine Predator Group is an open science lab that believes in transparent, reproducible science.  To that aim:
1. We keep lab notebooks to record what we did, learned, or produced each day. Can be physical notebooks, text files, Evernote, Jupyter notebooks, R Markdown notebooks, R blogdown, etc.
1. We do our data analysis in GitHub repositories in the @marine-predator-group organization to facilitate collaboration and sharing within the group.
1. We keep our raw data in the github repository related to the project, unless the data files are too large.
    1. We generally use a folder called "data" within the repository.  
    1. We store our raw data with metadata describing what’s in the file and what the columns mean
    1. If we clean the data, we often use a folder called something like "data-raw" and a folder called "data-clean" to differentiate data in its original form from data that has been manipulated.
    1. If we are using data downloaded from another data source, we often have a folder called "data_dl" for downloaded data, that is not tracked in GitHub. We include the data source in a README file for reproducibility. For large, downloaded datasets, it is ok to simply reference the dataset and provide some simple code for accessing that data from its home server (e.g. CoastWatch).
1. If (y)our data are too large to store on github, please store them on the group server (sixgill.fish.washington) in your own directory.
1. We back up our data in at least two places (beyond our computers). The cloud can be one site. An external harddrive can be another. You're welcome to backup to sixgill.fish.washington within your own directory.
1. We use scripts to process data, make models, do analyses, etc.
1. We publish git repositories through Zenodo upon publication of a manuscript.
1. Collaborative manuscripts are written in Overleaf, google drive, or via one of the R packages that faciliate combined text and code (e.g. drake or blogdown).
1. When matriculating, make sure all projects, code, papers, data, etc. are in the @marine-predator-group organization on GitHub and/or Google Drive.

# For group discussion and some trial & error
1. We generally make presentations in google slides so that other lab members can easily access useful graphics. However, CDB still uses Keynote. We should consider coalescing on an R-centric (or other open source method) for easy, reproducible slide generation and sharing.
