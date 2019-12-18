
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

Remember to make the few key changes to your notebook to start making it your own. For example, most sites have a `base_url` parameter in the config file as well as other personal information. 

As an example workflow and to leverage the modifications (from jekyll-now) that Steven has made...

1) Fork his repository associated with his notebook: https://github.com/sr320/sr320.github.io.   

2) Change the user name associated the repository name in the Settings.

3) Revise the config.xml file to include your own personal information 

4) Alter line 49 of `your_username.github.io/_layouts/default.html` so clicking on "admin" link takes you to your `_posts` directory.

5) Go to Disqus to set up comments for your website. Pick a page name, ignore instructions on adding code to your site. Complete registration. 

6) Go back to config.xml file and add your Disqus shortname. This will magically alter code so comments will show up for each posts. 

Note sometimes revisions take a few minutes to render on GitHub.

