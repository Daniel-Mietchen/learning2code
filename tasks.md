# About
In this file, I am collecting ideas that I consider doable for me in Python if I take some time to read up on details. 

Besides educating me about Python, they have some real-world application that I find useful, so if any of them meet your fancy, feel free to implement them or point me to a solution. 

If the resulting code works, you have helped solve a real problem (minor though it may be in light of all the major problems of the world), and thanks for that. If the code is open-source, I can use it to learn &mdash; thanks for that too. If the code is also openly licensed, I (and others) can actually reuse and adapt it to solve similar problems or to learn new things around the original one &mdash; special thanks for that!

# Topics
## Wikidata tools
### Import citation information
* [PMC lookup of publications on Zika, sorted by citation count](http://www.ebi.ac.uk/europepmc/webservices/rest/search?query=zika%20sort_cited:y)
* [PMC FTP service](https://www.ncbi.nlm.nih.gov/pmc/tools/ftp/)
   * has list of all PMCIDs in Open Subset
* [Europe PMC API call to download all citations for a given PMCID](http://www.ebi.ac.uk/europepmc/webservices/rest/PMC/PMC109351/citations/1/287/xml)
   * see [documentation](http://europepmc.org/RestfulWebService#cites)
   * [script for doing much the same thing via PMC](https://gist.github.com/mcfrank/c1ec74df1427278cbe53)
   * [script for searching dbVar](https://www.ncbi.nlm.nih.gov/dbvar/content/tools/entrez/) can probably be adapted easily to search PMC or other Entrez-listed databases
* [Wikidata Query Service API call to yield QID for a given PMCID](https://wdq.wmflabs.org/api?q=string%5B932:%22109351%22%5D)
* [Wikidata query for all items with a PMCID](https://query.wikidata.org/#SELECT%20%3Fitem%20%3Fpmcid%20WHERE%20%7B%0A%20%20%3Fitem%20wdt%3AP932%20%3Fpmcid%20.%0A%7D%20)

### Converting [JATS](http://jats.nlm.nih.gov/)/[TaxPub](https://github.com/tcatapano/TaxPub) to a format that [Quick Statements](http://tools.wmflabs.org/wikidata-todo/quick_statements.php) can ingest
* [Example XML file with description of 17 new species](http://phytokeys.pensoft.net/lib/ajax_srv/article_elements_srv.php?action=download_xml&item_id=5203)
* Tasks:
  1. Start Wikidata items for the authors of the paper
  1. Start Wikidata items for the paper itself, listing the authors accordingly
  1. Start Wikidata items for the species described in the paper, listing the relevant authors as taxon authority and the paper as a reference
* useful hints:
   * [Quickly Extract XML Data with Python](http://www.rdegges.com/quickly-extract-xml-data-with-python/)
     * some more examples [here](http://stackoverflow.com/questions/7691514/extracting-text-from-xml-using-python)
   * [Quick statements for journal articles and taxa](https://www.wikidata.org/wiki/User:Daniel_Mietchen/Quick_statements)

## LIGO
* repeat the [LIGO Jupyter analysis of GW150914](https://twitter.com/KyleCranmer/status/698240530900193282) for [GW151226](https://en.wikipedia.org/wiki/GW151226)
* modify the relevant figures and sound files, so they can be uploaded to Wikimedia Commons (see [Category:Gravitational wave events](https://commons.wikimedia.org/wiki/Category:Gravitational_wave_events) and [Category:WAV files](https://commons.wikimedia.org/wiki/Category:WAV_files)).
