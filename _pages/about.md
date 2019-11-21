---
permalink: /
title: "academicpages is a ready-to-fork GitHub Pages template for academic personal websites"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

### Credits

The 4xx and 6xx course will provide 4 design-credits both semesters. 
The 2xx level is 3 credits both semesters.

### Course Requirements

Admittance to this course requires approval from the instructor, to ensure the students in the course are sufficient diverse along a number of dimensions. To gain admittance, you must:

1. Be more excited about this course than any other academic endeavor for the year. Nobody is required to teach or take this course, and since so many people want to take it each year, preference is given to those that are most passionate about the material.
2. In practice, people commonly spend up to 20 hrs per week in this class, or more.  It is often rated one of the most challenging courses, so please consider that when making your course schedule. Priority will be given to students that certainly have room to be successful in the course.
3. For the 4xx and 6xx class, some background in numerical programming is required.
4. Because this course is based on team projects, entire teams are approved all at once. You can join the course slack channel here to chat with other potential team mates.
5. Send the CV and transcript of all members of your planned team to me for joint approval.


### Background

This course is based on my experience as an academic, and entrepreneur, an advisor, and an instructor. It is designed to be the best class you'll ever take. You will learn (by doing and getting feedback) the skills that I have found particularly useful in my endeavors. It will be organized into weekly sprints. Weekly progress will be reported documenting goals towards your team sprints, with sprint demo's to happen at the close of each sprint. Each team will be graded jointly on the basis of meeting the sprint goals, as well as providing clear and concise weekly progress reports.

The main "skills" you will learn in this class include:

- How to choose a project *significant* for the world, *feasible* for you, and that you are intrinsically motivated to complete (see [https://bitsandbrains.io/2018/08/31/sig-and-feas.html]).
- How to scope work so that you can achieve weekly progress towards quarterly goals (see [https://www.mindtools.com/pages/article/smart-goals.htm]).
- How to effectively communicate technical content.
- How to generate publication quality figures (see [figure checklist](https://bitsandbrains.io/2018/09/08/figures.html)).
- How to complete a wide set of data science tasks, spanning from data wrangling to statistical modeling.
- How to peacefully and productively work with a diverse team of passionate individuals.


### Potential Projects

The set of approved open-source repositories to contribute to include:

- [scipy](https://www.scipy.org/scipylib/index.html)
- [sklearn](https://scikit-learn.org/stable/)
- [networkx](https://networkx.github.io/)
- [skimage](https://scikit-image.org/docs/dev/api/skimage.html)
- [dipy](https://dipy.org/)
- [mne](https://martinos.org/mne/stable/index.html)


### Datasets

This course requires some analysis of data, the only approved dataset is the 
 [https://healthybrainnetwork.org/](Healthy Brain Network).  If for some reason you believe your tool cannot be applied to these data, please discuss with the TA.

 ### [Code of Conduct](https://neurodata.io/about/agreements/#respect)



A data-driven personal website
======
Like many other Jekyll-based GitHub Pages templates, academicpages makes you separate the website's content from its form. The content & metadata of your website are in structured markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over -- just be sure to save the markdown files! Finally, you can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
2. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 
3. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
4. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
5. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
6. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the academicpages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring academicpages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.
