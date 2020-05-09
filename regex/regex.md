# About

This file helps me collect resources useful to use (i.e. create, analyze and understand) regular expressions.

# Websites

* [Regexper](https://regexper.com/#%28%5CW%5Cw%7B1%7D%5CW%29%7B1%2C%7D)
* [Regex101](https://regex101.com/r/cO8lqs/6)

# Interesting features

* [RegExp $1, $2, $3, $4, $5, $6, $7, $8, $9](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp/n)
* [comments for regexes](https://stackoverflow.com/a/863170/446855)

# Examples that work for me

* [a string of any length containing any characters but which must contain 21 commas](https://stackoverflow.com/questions/863125/regular-expression-to-count-number-of-commas-in-a-string)

# Examples that do not (or only partially) work for me

* [author name strings without one or more initials](https://query.wikidata.org/#PREFIX%20organization%3A%20%20%20%20%20%20%20%20%20%20%20%3Chttp%3A%2F%2Fwww.wikidata.org%2Fentity%2FQ1150437%3E%0A%0ASELECT%0A%20%20DISTINCT%20%3Fauthor_name%0A%0A%20%20%23%20Number%20of%20works%20with%20the%20%3Fauthor_name%20string%0A%20%20%3Fcount%0A%0A%20%20%3Fauthor%20%0A%0A%23%20Build%20URL%20to%20the%20Author%20disambiguator%20tool%20for%20a%20given%20author%20name%20string%20and%20a%20coauthor%20associated%20with%20the%20institution%0A%20%20%28CONCAT%28%0A%20%20%20%20%20%20%22https%3A%2F%2Ftools.wmflabs.org%2Fauthor-disambiguator%2F%3Fdoit%3DLook%2Bfor%2Bauthor%26name%3D%22%2C%0A%20%20%20%20%20%20ENCODE_FOR_URI%28%3Fauthor_name%20%29%2C%20%22%26filter%3Dwdt%253AP50%2Bwd%253A%22%2C%20%3Fqid%20%29%20AS%20%3Fresolver_url%29%0A%20%0AWHERE%20%7B%0A%20%20SELECT%20DISTINCT%20%3Fauthor_name%20%28COUNT%28DISTINCT%20%3Fwork%29%20as%20%3Fcount%29%20%3Fauthor%20%28REPLACE%28STR%28%3Fauthor%29%2C%20%22.%2aQ%22%2C%20%22Q%22%29%20AS%20%3Fqid%29%20WHERE%20%7B%0A%20%20%20%20%7B%20%3Fauthor%20wdt%3AP108%20%2F%20wdt%3AP361%2a%20organization%3A%20.%7D%0A%20%20%20%20UNION%0A%20%20%20%20%7B%20%3Fauthor%20wdt%3AP463%20%2F%20wdt%3AP361%2a%20organization%3A%20.%7D%0A%20%20%20%20UNION%0A%20%20%20%20%7B%20%3Fauthor%20wdt%3AP1416%20%2F%20wdt%3AP361%2a%20organization%3A%20.%7D%0A%0A%20%20%20%20%3Fwork%20wdt%3AP50%20%3Fauthor%20%3B%20wdt%3AP2093%20%3Fauthor_name%20.%0A%20FILTER%28%21regex%20%28LCASE%28%3Fauthor_name%29%2C%20%22%5C%5CW%5C%5Cw%7B1%7D%5C%5CW%22%29%29.%0A%23%20FILTER%28%21CONTAINS%28LCASE%28%3Fauthor_name%29%2C%20%22.%22%29%29%0A%0A%20%20%7D%0A%20%20GROUP%20BY%20%3Fauthor_name%20%3Fcount%20%3Fauthor%20%3Fqid%0A%20%20HAVING%20%28%3Fcount%20%3E%204%29%0A%23%20%20%20%20%20%20%20%20%20%20%20LIMIT%202000%0A%7D%0AORDER%20BY%20DESC%28%3Fcount%29%20%0ALIMIT%20100%0A)
  - I used ```\W\w{1}\W```, which should match "non-word ==> word of length 1 ==> non-word)
  - Filtering for just strings containing a dot does most of what I want but feals untidy
  - Here are a few more variations that I tried
    - ```FILTER(!regex (LCASE(?string), "(\\W\\w{1}\\W){1,}")).```
    - ```FILTER(!regex (LCASE(?string), ".*(\\W\\w{1}\\W){1,}.*")).```
    - ```FILTER(!regex (LCASE(?string), "^.*?(\\b\\w{1}\\b).*$")).``` <== that actually [worked](https://query.wikidata.org/#SELECT%20%3Fstring%0AWHERE%20%7B%0A%20%20VALUES%20%3Fstring%20%7B%20%22J.%20Smith%22%20%22J%20Smith%22%20%22Smith%20J%22%20%22Jane%20A.%20B.%20C.%20Smith%22%20%22Jane%20Smith%22%20%22Jane%20Anne%20Smith%22%20%7D%0A%20%20FILTER%28%21regex%20%28LCASE%28%3Fstring%29%2C%20%22%5E.%2a%3F%28%5C%5Cb%5C%5Cw%7B1%7D%5C%5Cb%29.%2a%24%22%29%29.%0A%7D%0A), but I am leaving these examples in here because I do not fully understand why this one worked and the others did not
