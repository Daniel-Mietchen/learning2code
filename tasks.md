# About
In this file, I am collecting ideas that I consider doable for me in Python if I take some time to read up on details. 

Besides educating me about Python, they have some real-world application that I find useful, so if any of them meet your fancy, feel free to implement them or point me to a solution. 

If the resulting code works, you have helped solve a real problem (minor though it may be in light of all the major problems of the world), and thanks for that. If the code is open-source, I can use it to learn &mdash; thanks for that too. If the code is also openly licensed, I (and others) can actually reuse and adapt it to solve similar problems or to learn new things around the original one &mdash; special thanks for that!

# Topics
## Converting JATS/TaxPub to a format that [Quick Statements](http://tools.wmflabs.org/wikidata-todo/quick_statements.php) can ingest
* [Example XML file with description of 17 new species](http://phytokeys.pensoft.net/lib/ajax_srv/article_elements_srv.php?action=download_xml&item_id=5203)
* Task 1: Start Wikidata items for the authors of the paper
* Task 2: Start Wikidata items for the paper itself, listing the authors accordingly
* Task 3: Start Wikidata items for the species described in the paper, listing the relevant authors as taxon authority and the paper as a reference
* useful hints:
   * [Quickly Extract XML Data with Python](http://www.rdegges.com/quickly-extract-xml-data-with-python/)
