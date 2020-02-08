
### Research Notebooks

Keeping track of your work, including successes *and* failures, is a key part of doing science. To that end, MPG members are required to maintain a research notebook. You are free to choose exactly what works best for you, but we've compiled some best practices below based on our experiences. The landscape of tools for this is constantly changing, if you find a new or better tool that you think we should know about, provide your comments as an [issue(https://github.com/marine-predators-group/how-we-work/issues) or, for relatively minor changes (e.g. adding examples), feel free to directly edit this page.

## Key considerations for your notebook include:

An online research notebook is required of all lab members. Entries need to be organized by date and in reverse chronological order. 

### Make sure it is reproducible
Document in a fashion where someone could replicate your work.

### Document daily
A record of your work should be published the day of activity. Yep, daily! Even if you feel like you did nothing, post <em>something</em> to describe what you did that day. Did you read some papers? Great! Make a post that lists the papers you read. Did you spend all day searching the web? Also great! Make a post about what you were searching for and how successful you were in finding what you wanted.

### Maintain a backup
Have a copy of your notebook in another location. This could be done in several ways.
- composing in text editor and hosting on GitHub (probably the best/easiest solution)
- using IFTTT to post/save entries elsewhere
- run script (i.e. wget) to archive contents

Periodically, you will be asked to show where your backup is and demonstrate that it is functional.

### Platforms

A lot of people like to use a [jekyll-now](https://github.com/barryclark/jekyll-now) based notebook (hosted on GitHub). Several good examples come from SAFS and friends, including [Laura's Notebook](laurahspencer.github.io/LabNotebook/), [Steven's Notebook](sr320.github.io), [Yaamini's Notebook](yaaminiv.github.io) and [Holly's notebook](https://github.com/hputnam/Putnam_Lab_Notebook).

However, I want my notebook to be easily search-able with prominent dates of each post. I think [Sam's notebook](https://github.com/RobertsLab/sams-notebook) fills those needs pretty well.

Of course there are many other options including [blogdown](https://www.r-bloggers.com/setting-up-our-blog-with-rstudio-and-blogdown-i-creating-the-blog/) with Rstudio.


### Guide to creating a notebook:

You can readily duplicate any of the excellent examples above by forking the git repo the notebook is based on. Often, other pretty minor setup is required. See the excellent instructions for [jekyll-now](https://github.com/barryclark/jekyll-now) as a starting point.

I also find [Rajat Shah's](https://shahrajat.com/2016-06-22-install-jekyll-subdirectory-blog-github-pages/) tutorial particularly good. [Cam's notebook](https://marine-predators-group.github.io/cams-nb/) (hosted in this [repo](https://github.com/marine-predators-group/cams-nb)) is created following these instructions except I've forked the actual pages and content from [Sam's notebook](https://github.com/RobertsLab/sams-notebook) instead of cloning Rajat's example `blog.git`. This [thread](https://stackoverflow.com/questions/23417062/getting-jekyll-running-just-for-a-subdirectory-on-github?rq=1) on stackoverflow is also useful.

Remember there are a few key changes to make in order to make your notebook your own. For example, most sites have a `base_url` parameter in the config file as well as other personal information. 

As an example workflow and to leverage the modifications (from jekyll-now) that Steven has made...

1) Either duplicate one of the other group members repos:
https://help.github.com/en/github/creating-cloning-and-archiving-repositories/duplicating-a-repository#mirroring-a-repository

Or (recommended) fork a notebook repo from elsewhere. See individual nbs for the source of their fork. This is the recommended method because this allows creating pull requests between the two repositories (e.g. in order to update one from the other easily), although changes between two repos owned by the same account (mpg) are possible but slightly more technical. You could start by forking Steven's notebook repo, for example: https://github.com/sr320/sr320.github.io.

2) Right below the <code> tab you will see your repo name text. To the right of that is an edit button. Choose that and paste in the **github pages address** for your new notebook website. Note: this is NOT the address to your github repo!! It will look something like:
https://marine-predators-group.github.io/cams-nb/ where the last part is your repo name.

3) Now create a local copy of this notebook repo so you can make and push changes to your notebook. Create an R project based on your repo (in RStudio go New Project -> follow the prompts for using GitHub version control for existing directory which is your repo). 

4) Once you have the GitHub repo locally, start making changes like add some images to the ./images directory, change the personal info in the _config.yml file, etc. Once you’ve made a few changes, commit those and push to GitHub. Then you’ll see those changes reflected in the rendered website, although note that sometimes this takes a few mins for the changes to update on the website. 

5) To make a new notebook entry, copy one of the existing .md files in the ./posts directory, save as a new .md, and start building a markdown entry for your notebook. Easy!


Setup Disqus if you care:
x) Go to Disqus to set up comments for your website. Pick a page name, ignore instructions on adding code to your site. Complete registration. 

x) Go back to config.xml file and add your Disqus shortname. This will magically alter code so comments will show up for each posts. 

Note sometimes revisions take a few minutes to render on GitHub.

