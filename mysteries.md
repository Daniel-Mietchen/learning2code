# About

This file collects things I stumbled upon and did not fully grasp, at least not at first sight. If you know of resources with good explanations, I would appreciate notice.

# Python

* [::](https://docs.python.org/release/2.3.5/whatsnew/section-slices.html) ("stepping slices")
* The philosophical differences between Python 2 and 3, and their practical implications as to whether a given piece of code from one will work in the other or not, and why
  - [The key differences between Python 2.7.x and Python 3.x with examples](http://sebastianraschka.com/Articles/2014_python_2_3_key_diff.html)
* how to find out
  - what modules exist for doing a certain task
    - say, reading in some data available in JSON
  - what a particular module does
    - e.g. [Beautiful Soup](https://pypi.python.org/pypi/beautifulsoup4)
  - what the objects within a particular module do
    - e.g. after having imported pandas, I can find out by tab completion that there is an object pandas.read_json() in there, but it's not immediately clear what this does 
      - try ```pandas.read_json?``` , which should provide some help message and explain the object type
* how best to document dependencies upfront and explicitly
  - think [requirements.txt](https://pip.pypa.io/en/stable/user_guide/#requirements-files)

# SPARQL

* moved to [dedicated file](SPARQL/sparql.md)

# Regexes

* [regex tester](https://regex101.com/)
* [regex lookaround](http://www.regular-expressions.info/lookaround.html)

# CSS

* [Wikidata logo in CSS](https://twitter.com/LucasWerkmeistr/status/980428984918921216)
  - > HTML:
```HTML
<div id="stage">
  <div></div>
</div>
```
  - > CSS: 
```CSS
  #stage div {
  --red: #990000;
  --green: #339966;
  --blue: #006699;
  --white: #FFFFFF;
  --height: 85px;
  --text-height: 25px;
  --short-stripe: 5px;
  --long-stripe: 15px;
  --inter-stripe: 5px;
  --stripe-1-start: 0px;
  --stripe-1-end: calc(var(--stripe-1-start) + var(--short-stripe));
  --stripe-2-start: calc(var(--stripe-1-end) + var(--inter-stripe));
  --stripe-2-end: calc(var(--stripe-2-start) + var(--long-stripe));
  --stripe-3-start: calc(var(--stripe-2-end) + var(--inter-stripe));
  --stripe-3-end: calc(var(--stripe-3-start) + var(--long-stripe));
  --stripe-4-start: calc(var(--stripe-3-end) + var(--inter-stripe));
  --stripe-4-end: calc(var(--stripe-4-start) + var(--short-stripe));
  --stripe-5-start: calc(var(--stripe-4-end) + var(--inter-stripe));
  --stripe-5-end: calc(var(--stripe-5-start) + var(--short-stripe));
  --stripe-6-start: calc(var(--stripe-5-end) + var(--inter-stripe));
  --stripe-6-end: calc(var(--stripe-6-start) + var(--long-stripe));
  --stripe-7-start: calc(var(--stripe-6-end) + var(--inter-stripe));
  --stripe-7-end: calc(var(--stripe-7-start) + var(--short-stripe));
  --stripe-8-start: calc(var(--stripe-7-end) + var(--inter-stripe));
  --stripe-8-end: calc(var(--stripe-8-start) + var(--long-stripe));
  --stripe-9-start: calc(var(--stripe-8-end) + var(--inter-stripe));
  --stripe-9-end: calc(var(--stripe-9-start) + var(--short-stripe));
  --stripe-10-start: calc(var(--stripe-9-end) + var(--inter-stripe));
  --stripe-10-end: calc(var(--stripe-10-start) + var(--short-stripe));
  
  position: relative;
  top: calc(50% - (var(--height) + var(--text-height)) / 2);
  left: calc(50% - var(--stripe-10-end)/2);
  width: var(--stripe-10-end);
  height: var(--height);
  background: linear-gradient(
    to right,
    var(--red) var(--stripe-1-start),
    var(--red) var(--stripe-1-end),
    var(--white) var(--stripe-1-end),
    var(--white) var(--stripe-2-start),
    var(--red) var(--stripe-2-start),
    var(--red) var(--stripe-2-end),
    var(--white) var(--stripe-2-end),
    var(--white) var(--stripe-3-start),
    var(--red) var(--stripe-3-start),
    var(--red) var(--stripe-3-end),
    var(--white) var(--stripe-3-end),
    var(--white) var(--stripe-4-start),
    var(--green) var(--stripe-4-start),
    var(--green) var(--stripe-4-end),
    var(--white) var(--stripe-4-end),
    var(--white) var(--stripe-5-start),
    var(--green) var(--stripe-5-start),
    var(--green) var(--stripe-5-end),
    var(--white) var(--stripe-5-end),
    var(--white) var(--stripe-6-start),
    var(--blue) var(--stripe-6-start),
    var(--blue) var(--stripe-6-end),
    var(--white) var(--stripe-6-end),
    var(--white) var(--stripe-7-start),
    var(--blue) var(--stripe-7-start),
    var(--blue) var(--stripe-7-end),
    var(--white) var(--stripe-7-end),
    var(--white) var(--stripe-8-start),
    var(--blue) var(--stripe-8-start),
    var(--blue) var(--stripe-8-end),
    var(--white) var(--stripe-8-end),
    var(--white) var(--stripe-9-start),
    var(--green) var(--stripe-9-start),
    var(--green) var(--stripe-9-end),
    var(--white) var(--stripe-9-end),
    var(--white) var(--stripe-10-start),
    var(--green) var(--stripe-10-start),
    var(--green) var(--stripe-10-end),
    var(--white) var(--stripe-10-end)
  );
}

#stage div::after {
  content: "Wikidata";
  text-transform: uppercase;
  color: #484848;
  position: absolute;
  font-family: "Bitstream Vera Sans", "sans-serif";
  font-weight: bold;
  font-size: var(--text-height);
  text-align: center;
  top: calc(var(--height) + var(--inter-stripe));
  width: var(--stripe-10-end);
}

/* --------- setup --------- */
#stage {
  background: white;
  width: 300px;
  height: 300px;
  position: absolute;
  top: 50%;
  left: 50%;
  margin: -250px 0 0 -250px;
}
body {
  background: #222;
}
```
