# About
This file collects things I stumbled upon and did not fully grasp, at least not at first sight.

# Python
* [::](https://docs.python.org/release/2.3.5/whatsnew/section-slices.html) ("stepping slices")
* The philosophical differences between Python 2 and 3, and their practical implications as to whether a given piece of code from one will work in the other or not, and why

# SPARQL syntax
* [.](https://data-gov.tw.rpi.edu/wiki/How_to_use_SPARQL#Query_syntax)
* [p:](https://query.wikidata.org/#select%20%3Fitem%20%3Fseriesordinal%20%3Fauthoritem%20where%20%7B%0A%20%20%3Fitem%20p%3AP2093%20%3Fauthorstring%20.%0A%20%20%3Fitem%20p%3AP50%20%3Fauthoritem%20.%0A%20%20%3Fauthoritem%20pq%3AP1545%20%3Fseriesordinal%20.%0A%20%20%3Fauthorstring%20pq%3AP1545%20%3Fseriesordinal%20.%0A%7D) (as opposed to "wdt:")
* [ps:](https://www.wikidata.org/wiki/Wikidata:SPARQL_query_service/queries/examples#Number_of_handed_out_academy_awards_per_award_type)
* [pq:](https://www.wikidata.org/wiki/Wikidata:SPARQL_query_service/queries/examples#Number_of_handed_out_academy_awards_per_award_type)

# SPARQL queries that did not work for me (at least not as expected)
* [duplicate series ordinal (P1545) for author string (P2093) statements](https://query.wikidata.org/#select%20%3Fitem%20%3Fseriesordinal%20where%20%7B%0A%20%20%3Fitem%20p%3AP50%20%3Fauthorstring%20%3B%0A%20%20%20%20%20%20%20%20p%3AP50%20%3Fauthorstring2%20.%0A%20%20%3Fauthorstring%20pq%3AP1545%20%3Fseriesordinal%20.%0A%20%20%3Fauthorstring2%20pq%3AP1545%20%3Fseriesordinal%20.%0A%7D)
  - [a similar query, with similar issues](https://query.wikidata.org/#select%20%3Fitem%20%3Fseriesordinal%20%3Fauthoritem%20where%20%7B%0A%20%20%3Fitem%20p%3AP2093%20%3Fauthorstring%20.%0A%20%20%3Fitem%20p%3AP50%20%3Fauthoritem%20.%0A%20%20%3Fauthoritem%20pq%3AP1545%20%3Fseriesordinal%20.%0A%20%20%3Fauthorstring%20pq%3AP1545%20%3Fseriesordinal%20.%0A%7D)
