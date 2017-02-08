# About

This file is my attempt to report on how I am learning the programming language Python. It complements [resources.md](https://github.com/Daniel-Mietchen/learning2code/blob/master/resources.md) by focusing on the process and circumstances of my learning as a way to help others in theirs. I does include some remarks on how my learning of Python triggered other learning experiences.

# Flash Grant

In late 2015, I was awarded one of the Shuttleworth Foundation's [Flash Grants](https://www.shuttleworthfoundation.org/flashgrants/). These are handed out twice a year to unsuspecting awardees upon nomination by [Shuttleworth Fellows](https://shuttleworthfoundation.org/fellows/) &mdash; in my case [Peter Murray-Rust](https://en.wikipedia.org/wiki/Peter_Murray-Rust), with whom I am sharing an interest in [open research](https://www.youtube.com/watch?v=LwW1-X3glak).

Initially, I thought I would use the freedom that the Flash Grant accorded to me to step up my efforts in learning [Python](https://www.python.org/), for which I had started this repo some months earlier as an attempt to document my progress (or the lack thereof). The [announcement](https://twitter.com/EvoMRI/status/668738865600032768) of the plan quickly brought about some useful [feedback](https://twitter.com/kirstie_j/status/668739834664587264) (which I followed and now agree with), so I was hopeful for doing my learning in public.

Expecting the [RIO launch](http://dx.doi.org/10.3897/rio.1.e7547) to consume most of my spare time in December (which it did) and wiki activities to continue for months to come (most notably the [Open Access Signalling](https://en.wikipedia.org/wiki/Wikipedia:WikiProject_Open_Access/Signalling_OA-ness) project, the [Open Access Media Importer](https://commons.wikimedia.org/wiki/User:Open_Access_Media_Importer_Bot) and [bibliographic metadata on Wikidata](https://www.wikidata.org/wiki/Template:Bibliographical_properties)), I earmarked some time in late January and early February specifically for diving deeper into Python.

When that time came, the [Zika outbreak](https://en.wikipedia.org/wiki/2015%E2%80%9316_Zika_virus_epidemic) had begun to emerge as a serious public health issue. I had been [keeping track](https://github.com/Daniel-Mietchen/datascience/blob/master/emergency-response.md) for a while of cases where emergency situations like epidemics or earthquakes had triggered open and collaborative responses, so I began to wonder what open knowledge initiatives could do about Zika.

The simplest answer to that was of course to read up on the virus, its effects on humans and potential response measures. Aside from access issues, this was initially relatively straightforward: since the first description of the virus in 1952, there had been just a bit over a hundred papers specifically on Zika. I started to track them via [Wikidata](https://query.wikidata.org/#SELECT%20%3Fitem%20WHERE%20{%20{%20%3Fitem%20wdt%3AP921%20wd%3AQ202864%20.%20}%20UNION%20{%20%3Fitem%20wdt%3AP921%20wd%3AQ8071861%20.%20}%20}), experimented with the [timeline feature](https://tools.wmflabs.org/wikidata-timeline/#/timeline?query=CLAIM%5B921:202864%5D%20OR%20CLAIM%5B921:8071861%5D) and began to [add](https://en.wikipedia.org/w/index.php?title=Zika_virus&type=revision&diff=701345863&oldid=701318605) references to Zika-related wiki pages.

Soon thereafter, I stumbled across the [ZikaOpen hashtag](https://twitter.com/collabchem/status/692762591706365953) on Twitter. This brought me [together with others](http://dx.doi.org/10.12688/f1000research.8013.1) who wanted to address the outbreak using open-science approaches, and I shifted my spare time attention from Python to Zika, though with some hope that there might be occasions to combine the two somehow.

In the meantime, I am continuing to dive into Python whenever there is an opportunity to do so in the framework of other activities, e.g. while trying to understand [this simulation](http://www.spatial-epi.com/zika-virus-vector-control-2/) of the spread of the virus or [this reanalysis of open Zika data](http://nbviewer.jupyter.org/github/maayanlab/Zika-RNAseq-Pipeline/blob/master/Zika.ipynb)). I made some reasonable progress over the last few months in this regard, which can be traced (with some effort) through the repo's [version history](https://github.com/Daniel-Mietchen/learning2code/commits/master), but still prefer command-line tools like sed and awk for simple data processing and am shying away from anything more complex. While I am becoming quicker at understanding Python codes and spotting or fixing simple bugs, I am still hesitating to write something really on my own, and I am still lacking an overview over the huge and rich landscape of existing [Python libraries](https://pypi.python.org/pypi?%3Aaction=index).

My professional and volunteer activities (especially those around Wikimedia projects) are regularly pushing me towards deepening my technical knowledge, be this in terms of familiarizing myself with [JATS XML](https://www.ncbi.nlm.nih.gov/books/NBK159964/), [SPARQL](https://query.wikidata.org/#PREFIX%20wd%3A%20%3Chttp%3A%2F%2Fwww.wikidata.org%2Fentity%2F%3E%0APREFIX%20wdt%3A%20%3Chttp%3A%2F%2Fwww.wikidata.org%2Fprop%2Fdirect%2F%3E%0APREFIX%20prov%3A%20%3Chttp%3A%2F%2Fwww.w3.org%2Fns%2Fprov%23%3E%0APREFIX%20pr%3A%20%3Chttp%3A%2F%2Fwww.wikidata.org%2Fprop%2Freference%2F%3E%0A%0ASELECT%20%3Fstatement%20%3FPMID%20%3FPMCID%20WHERE%20%7B%0A%20%20%3Fstatement%20prov%3AwasDerivedFrom%2Fpr%3AP248%20%3Fpaper%20.%0A%20%20%3Fpaper%20wdt%3AP31%20wd%3AQ13442814%20.%0A%20%20OPTIONAL%20%7B%20%3Fpaper%20wdt%3AP698%20%3FPMID%20.%20%7D%0A%20%20OPTIONAL%20%7B%20%3Fpaper%20wdt%3AP932%20%3FPMCID%20.%20%7D%0A%20%20FILTER%20%28BOUND%28%3FPMID%29%29%0A%7D), [Lua](https://www.wikidata.org/w/index.php?title=Module:Cite&action=edit) or even going back to dealing with [regexes](https://www.wikidata.org/w/index.php?title=Property_talk:P304&diff=prev&oldid=340705527) (with which I was more familiar ten years ago when I was dabbling in Perl). 

While I am not specifically watching out for occasions to learn and/ or use Python, such opportunities present themselves on a regular basis, and I gladly jump on them. For instance, the [Open Science Fellows Program](https://meta.wikimedia.org/wiki/Wikimedia_Deutschland/Open_Science_Fellows_Program) run by Wikimedia Germany and the Stifterverband offers a group of [young scientists from various backgrounds](https://wikimedia.de/wiki/BildungWissenschaftKultur/Fellowprogramm/Fellows) the opportunity to explore open science by trying it out for some aspect of their research, with guidance not just from their discipline-specific supervisors but also from a group of [mentors](https://wikimedia.de/wiki/BildungWissenschaftKultur/Fellowprogramm/MentorInnen) experienced with open science. One of my fellows in this context is [Nicholas Schmelling](https://twitter.com/derschmelling), who uses a Python-focused approach to studying the [evolution of circadian clocks](https://github.com/schmelling/clock_evo). Simply by reviewing and testing what he has done and by discussing what comes next, I will be exposed to Python in multiple ways.

# Prehistory

I became interested in programming languages in the mid 1980s. At the time, I did not know anyone who owned a computer, so the interest was largely theoretical, i.e. I studied computer programs &mdash; mostly BASIC &mdash much the same way I would study a mathematical problem or some aspect of natural languages: by reading about them on paper, writing things down on paper, striking stuff out, and iterating. 

Likewise, none of my schools till then had had a computer, but by being active in math circles and asking around, I got to know a few schools that did. One of them was actually within my reach, and they were kind enough to allow a friend and me to come over there for two hours every other week to play around with a [KC-85/2](https://en.wikipedia.org/wiki/KC_85). Initially, what we did was indeed mostly playing (e.g. hunting treasures within some pyramids), through which we discovered some basic graphics and that we could fiddle around with them, since their source code was available to and editable by us. We also did some math, e.g. wrote some scripts to have the computer calculate some numbers for which we had (or were trying to get) analytical solutions, and we experimented with plotting functions, though we quickly hit limits there in terms of display and memory.

After the [wall](https://en.wikipedia.org/wiki/Berlin_Wall) had come down, my interactions with computers intensified considerably. By the mid-90s, BASIC wasn't very useful any more, but I had become reasonably fluent in [Pascal](https://en.wikipedia.org/wiki/Pascal_(programming_language)), which I was still using around 2000 towards the end of my studies of biophysics, primarily to control lab equipment and for simple programmatic calculations as part of other experimental workflows. I complemented that with some basic mathematical modeling in [Maple](https://en.wikipedia.org/wiki/Maple_(software)), which is similar in style to Pascal.

My PhD had a focus on experimental methodology, and the existing tools for handling the resulting data (mainly [ImageJ](http://imagej.net/), written in [Java](https://en.wikipedia.org/wiki/Java_(programming_language)) were usually good enough for my purposes, so that I only rarely had to do coding that went much beyond customizing.

I kept the experimental focus for my first postdoc, but the preparation and analysis of the experiments involved a decent amount of scripting, particularly in [Perl](https://en.wikipedia.org/wiki/Perl) and [Bash](https://en.wikipedia.org/wiki/Bash_(Unix_shell)) as well as through tools like [Lipsia](http://static.cbs.mpg.de/lipsia/), [Praat](https://en.wikipedia.org/wiki/Praat) and [MATLAB](https://en.wikipedia.org/wiki/MATLAB), all of which are largely written in [C](https://en.wikipedia.org/wiki/C_(programming_language)) and [C++](https://en.wikipedia.org/wiki/C%2B%2B), with which I was thus becoming more familiar too.

My second postdoc lost its initially foreseen experimental component early on, so computation via a combination of shell scripts, C and MATLAB became central, though I was again mostly customizing or adapting code that others had written, and I ended up doing lots of things manually for which no good automated solution was available. It was around that time that I first saw [version control](https://en.wikipedia.org/wiki/Version_control) (a concept that I had already become familiar with by contributing to Wikipedia) used systematically in the context of developing scientific software.

# Notes

* Version control: wikis, svn, git, GitHub
* MATLAB
  - frustration with license limitations
* Pywikibot
  * e.g. [Wikidata:Database reports/User preferences/Configuration](https://www.wikidata.org/wiki/Wikidata:Database_reports/User_preferences/Configuration)
* Software Carpentry
* [Sage](http://www.sagemath.org/)
  * seen [here](http://ways.org/en/node/1078)
* "I'm eyeing R"
* Python
* StackOverflow
* IPython
* Mybinder
  * [blog post by Titus Brown](http://ivory.idyll.org/blog//2016-mybinder.html)
* Flash Grant
* Anaconda
* Deepsense
* codeschool
* Pineapple
* hack.summit()
* pluralsight
* [LIGO data](https://losc.ligo.org/events/GW150914/)
   * [Jupyter notebook](https://losc.ligo.org/s/events/GW150914/GW150914_tutorial.ipynb) (in Python 2)
   * [mbinder version](http://mybinder.org/repo/cranmer/ligo-binder)
     * [seaborn error](http://stackoverflow.com/questions/33451260/cannot-import-seaborn)
       * solved by adding a requirements.txt file with "seaborn" as content, as per [this example](https://github.com/binder-project/example-requirements/blob/master/requirements.txt)
       * potentially solvable by editing the Docker file
     * discovered [IPython Parallel](https://github.com/ipython/ipyparallel)
     * [useful comments on mybinder](http://blog.ouseful.info/2015/10/31/running-github-hosted-jupyter-previously-ipython-notebooks-as-online-applications/)
   * [run it on mobile](https://twitter.com/KyleCranmer/status/698240530900193282)
* Scratch
* SPARQL
* Kunal Mehta [wrote](https://meta.wikimedia.org/wiki/Affiliate-selected_Board_seats/2016/Nominations/Kunal_Mehta) "I learned about Pywikibot, and self-taught myself Python using [Wikibooks](https://en.wikibooks.org/wiki/Non-Programmer's_Tutorial_for_Python_2.6)."
   * [Category:Python programming language](https://en.wikibooks.org/wiki/Category:Python_programming_language)
* Yuvi Panda started [Pywikibot: A Web Shell (PAWS)](https://www.mediawiki.org/wiki/Manual:Pywikibot/PAWS)
* When searching for he LIGO Jupyter notebook, I came across [this discussion](https://news.ycombinator.com/item?id=11094009), which brought me to the followwing great video
* [A Better Default Colormap for Matplotlib](https://www.youtube.com/watch?v=xAoljeRJ3lU)
   * [viscm](https://github.com/matplotlib/viscm)
   * [viridis](https://bids.github.io/colormap/)
* [FutureLearn course](https://www.futurelearn.com/courses/learn-to-code)?
* [Data science intro for math/phys background](http://p.migdal.pl/2016/03/15/data-science-intro-for-math-phys-background.html)
* [Running Executable Jupyter/IPython Notebooks Directly from Github With Binder](http://blog.ouseful.info/2015/10/31/running-github-hosted-jupyter-previously-ipython-notebooks-as-online-applications/)
* [Community Data Science Workshops at University of Washington](http://wiki.communitydata.cc/Community_Data_Science_Workshops_%28Spring_2016%29)
* [datapackage-py](https://github.com/frictionlessdata/datapackage-py)
* [Python Challenge app](https://play.google.com/store/apps/details?id=sg.apps.garden.pythonchallenge)
* [Real-world data in a few minutes with Google Science Journal](http://nbviewer.jupyter.org/github/fperez/science-journal-demo/blob/master/Light%20data%20with%20Google%20Science%20Journal.ipynb)
* [Calico](https://www.projectcalico.org/)
* [Python Village at Rosalind](http://rosalind.info/problems/list-view/?location=python-village)
* [Jupyter notebooks on Azure](https://notebooks.azure.com/)
* ["live programming mode of Python Tutor, which continually runs and visualizes your code as you type"](http://pythontutor.com/live.html#mode=edit)
* [A gallery of interesting IPython Notebooks](https://github.com/ipython/ipython/wiki/A-gallery-of-interesting-IPython-Notebooks)
  * [data journalism example](https://github.com/BuzzFeedNews/2016-01-tennis-betting-analysis/blob/master/notebooks/tennis-analysis.ipynb)
* [Testing Jupyter Notebooks](http://blog.thedataincubator.com/2016/06/testing-jupyter-notebooks/)
* [Learn to Code for Data Analysis](https://blog.ouseful.info/2016/04/26/want-to-get-started-with-open-data-looking-for-an-introductory-programming-course/)
* [IBM's Big Data University](http://bigdatauniversity.com/)
  * [commentary in Forbes](http://www.forbes.com/sites/bernardmarr/2016/05/26/ibms-big-data-university-free-online-learning-with-over-400000-students/#34a7f86c452a)
* [10 Useful Python Data Visualization Libraries for Any Discipline](https://blog.modeanalytics.com/python-data-visualization-libraries/#DataScience)
  * with visualizations in [Mode](https://about.modeanalytics.com/python/) [notebooks](https://modeanalytics.com/modeanalytics/reports/60ec15dd7173/python)
  * useful links also in the comments, e.g. [Up and Down the Python Data and Web Visualization Stack](http://nbviewer.jupyter.org/gist/wrobstory/1eb8cb704a52d18b9ee8/Up%20and%20Down%20PyData%202014.ipynb) and [Overview of Python Visualization Tools](http://pbpython.com/visualization-tools-1.html)
* [Implementing your own recommender systems in Python](http://online.cambridgecoding.com/notebooks/eWReNYcAfB/implementing-your-own-recommender-systems-in-python-2)
* [File and Directory Operations Using Python](http://code.tutsplus.com/tutorials/file-and-directory-operations-using-python--cms-25817)
* [Beginning Python Programming](http://www.openbookproject.net/books/bpp4awd/index.html)
* [Code Academy: Learn](https://www.codecademy.com/learn)
* [Biopython](http://biopython.org/DIST/docs/tutorial/Tutorial.html)
* [A Reanalysis of Lung Tumor Incidence in Mice Induced By Inorganic Arsenic Exposure](https://github.com/DataSciBurgoon/arsenic_mouse_lung_tumor_reanalysis/blob/master/Is%20Waalkes%20Arsenic%20Control%20Tumor%20Incidence%20Different%20From%20Tokar's-.ipynb)
  * link to paper [from Twitter](https://doi.org/10.1007/s00204-016-1749-0)
* [Coconut](http://coconut-lang.org/)
  * "Coconut is a simple, elegant, Pythonic functional programming language that compiles to Python. Since all valid Python is valid Coconut, using Coconut will only extend and enhance what you're already capable of in Python."
* [Why You Should Learn Python](https://iluxonchik.github.io/why-you-should-learn-python/)
* [Teaching an AI to write Python code with Python code](http://www.benjamintd.com/blog/spynet/)
* [Using chat bots as a prototyping tool](https://github.com/ideo/stanley-bot)
* [Baidu open-sources Python-driven machine learning framework](http://www.infoworld.com/article/3114175/artificial-intelligence/baidu-open-sources-python-driven-machine-learning-framework.html)
  * [Overview](http://www.paddlepaddle.org/)
  * [Python wrapper](http://www.paddlepaddle.org/doc/ui/data_provider/pydataprovider2.html)
* [Parsing JSON from command line using Python](http://www.cambus.net/parsing-json-from-command-line-using-python/)
* [Wikidata Query in Jupyter notebook](https://twitter.com/WikidataFacts/status/806636466143109121)
* [Reproducible Research using Jupyter Notebooks: Curriculum Development Hackathon](https://github.com/Reproducible-Science-Curriculum/RR-Jupyter-Hackathon-Jan-2016/blob/master/Call-for-participation.md)
