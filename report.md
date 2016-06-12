In late 2015, I was awarded one of the Shuttleworth Foundation's [Flash Grants](https://www.shuttleworthfoundation.org/flashgrants/). These are handed out twice a year to unsuspecting awardees upon nomination by [Shuttleworth Fellows](https://shuttleworthfoundation.org/fellows/) &mdash; in my case [Peter Murray-Rust](https://en.wikipedia.org/wiki/Peter_Murray-Rust), with whom I am sharing an interest in [open research](https://www.youtube.com/watch?v=LwW1-X3glak).

Initially, I thought I would use the freedom that the Flash Grant accorded to me to step up my efforts in learning [Python](https://www.python.org/), for which I had started this repo some months earlier as an attempt to document my progress (or the lack thereof). The [announcement](https://twitter.com/EvoMRI/status/668738865600032768) of the plan quickly brought about some useful [feedback](https://twitter.com/kirstie_j/status/668739834664587264) (which I followed and now agree with), so I was hopeful for doing my learning in public.

Expecting the [RIO launch](http://dx.doi.org/10.3897/rio.1.e7547) to consume most of my spare time in December (which it did) and wiki activities to continue for months to come (most notably the [Open Access Signalling](https://en.wikipedia.org/wiki/Wikipedia:WikiProject_Open_Access/Signalling_OA-ness) project, the [Open Access Media Importer](https://commons.wikimedia.org/wiki/User:Open_Access_Media_Importer_Bot) and [bibliographic metadata on Wikidata](https://www.wikidata.org/wiki/Template:Bibliographical_properties)), I earmarked some time in late January and early February specifically for diving deeper into Python.

When that time came, the [Zika outbreak](https://en.wikipedia.org/wiki/2015%E2%80%9316_Zika_virus_epidemic) had begun to emerge as a serious public health issue. I had been [keeping track](https://github.com/Daniel-Mietchen/datascience/blob/master/emergency-response.md) for a while of cases where emergency situations like epidemics or earthquakes had triggered open and collaborative responses, so I began to wonder what open knowledge initiatives could do about Zika.

The simplest answer to that was of course to read up on the virus, its effects on humans and potential response measures. Aside from access issues, this was initially relatively straightforward: since the first description of the virus in 1952, there had been just a bit over a hundred papers specifically on Zika. I started to track them via [Wikidata](https://query.wikidata.org/#SELECT%20%3Fitem%20WHERE%20{%20{%20%3Fitem%20wdt%3AP921%20wd%3AQ202864%20.%20}%20UNION%20{%20%3Fitem%20wdt%3AP921%20wd%3AQ8071861%20.%20}%20}), experimented with the [timeline feature](https://tools.wmflabs.org/wikidata-timeline/#/timeline?query=CLAIM%5B921:202864%5D%20OR%20CLAIM%5B921:8071861%5D) and began to [add](https://en.wikipedia.org/w/index.php?title=Zika_virus&type=revision&diff=701345863&oldid=701318605) references to Zika-related wiki pages.

Soon thereafter, I stumbled across the [ZikaOpen hashtag](https://twitter.com/collabchem/status/692762591706365953) on Twitter. This brought me [together with others](http://dx.doi.org/10.12688/f1000research.8013.1) who wanted to address the outbreak using open-science approaches, and I shifted my spare time attention from Python to Zika, though with some hope that there might be occasions to combine the two somehow.




&mdash; many of my wiki activities had a Python or Zika spin already.

I made some reasonable progress over the last few months in this regard, which can be traced (with some effort) through the repo's [version history](https://github.com/Daniel-Mietchen/learning2code/commits/master), but 

Zika hackathon at Force 2016
wiki activities as a driver for acquiring technical knowledge
[JATS](https://www.ncbi.nlm.nih.gov/books/NBK159964/)
SPARQL
[Lua](https://www.wikidata.org/w/index.php?title=Module:Cite&action=edit)
[regexes](https://www.wikidata.org/w/index.php?title=Property_talk:P304&diff=prev&oldid=340705527)

# Notes
This file is my attempt to report on how I am learning the programming language Python. It complements [resources.md](https://github.com/Daniel-Mietchen/learning2code/blob/master/resources.md) by focusing on the process and circumstances of my learning as a way to help others in theirs. I will include some remarks on how my learning of Python triggered other learning experiences.

## Outline
* Prehistory: school till postdoc
* Version control: wikis, svn, git
* MATLAB
* Pywikibot
* Software Carpentry
* [Sage](http://www.sagemath.org/)
  * seen [here](http://ways.org/en/node/1078)
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
