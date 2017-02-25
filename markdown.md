# About

I'll be using this file to play around with Markdown features, specifically with [GitHub-flavoured Markdown](https://guides.github.com/features/mastering-markdown/).

# Background

For background on Markdown, see

- https://en.wikipedia.org/wiki/Markdown
- https://help.github.com/articles/about-writing-and-formatting-on-github/
- https://help.github.com/articles/working-with-advanced-formatting/
- http://www.markdowntutorial.com/


# Generating a table of Contents for a given Markdown file

This does not seem to be part of standard Markdown, so various ways are being explored to achieve that functionality, e.g.

- https://github.com/jonschlinkert/markdown-toc
- https://pythonhosted.org/Markdown/extensions/toc.html


# Images in tables

* This is not mentioned in any of the sources listed in the Background section
* There is a discussion about it at http://stackoverflow.com/questions/255170/markdown-and-image-alignment but none of the options discussed there worked for me here.
* Includes text and images, but all under CC0/ Public Domain


## Test 1

| We invite you, whether you're in London or afar, to a weekend of learning, making, and doing to advance Open Research Data. The event is hosted by [SPARC](https://sparcopen.org/) and the [NIH](https://nih.gov/) as part of an international celebration for Open Data Day.

At its heart, Open Research Data is about making it easy for you and others to see, use and share data (to find out more, read [this](https://sparcopen.org/open-data/)). This simple idea is powering some of the largest [breakthroughs](https://sparcopen.org/impact-story/human-genome-project/) of our time, and our event aims to celebrate and accelerate the power of Open Research Data.

We invite you, whether new or old to Open Research Data, scholar or citizen, in London or across the globe, to join us for this weekend to make, hack, contribute, try, teach, design, test, learn (or just about anything!) in the name of Open Research Data.

In London, we'll provide fast wifi, power (both for your laptops and your bodies) and a program that will spark ideas and collaborations for the weekend.

If you can't make it to London, join us online from wherever you are.  | [Individual data points](https://upload.wikimedia.org/wikipedia/commons/4/40/Dews...%28byNithyaRamanujam%29.jpg)  |
|------|---|
|We invite you, whether you're in London or afar, to a weekend of learning, making, and doing to advance Open Research Data. The event is hosted by [SPARC](https://sparcopen.org/) and the [NIH](https://nih.gov/) as part of an international celebration for Open Data Day.|[Individual data points](https://upload.wikimedia.org/wikipedia/commons/4/40/Dews...%28byNithyaRamanujam%29.jpg) |

At its heart, Open Research Data is about making it easy for you and others to see, use and share data (to find out more, read [this](https://sparcopen.org/open-data/)). This simple idea is powering some of the largest [breakthroughs](https://sparcopen.org/impact-story/human-genome-project/) of our time, and our event aims to celebrate and accelerate the power of Open Research Data.

We invite you, whether new or old to Open Research Data, scholar or citizen, in London or across the globe, to join us for this weekend to make, hack, contribute, try, teach, design, test, learn (or just about anything!) in the name of Open Research Data.

In London, we'll provide fast wifi, power (both for your laptops and your bodies) and a program that will spark ideas and collaborations for the weekend.

If you can't make it to London, join us online from wherever you are. 

## Test 2

| Option | Description |
| ------ | ----------- |
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |

## Test 3

| ![An image](https://upload.wikimedia.org/wikipedia/commons/4/40/Dews...%28byNithyaRamanujam%29.jpg) | Try this out!  |
|-|-|

## Test 4

| test | ![Sandbox data visualization](https://upload.wikimedia.org/wikipedia/commons/2/2e/Sandbox_with_interactive_projection_at_31c3.jpg) |

## Test 5

| test | ![Sandbox data visualization](https://upload.wikimedia.org/wikipedia/commons/thumb/2/2e/Sandbox_with_interactive_projection_at_31c3.jpg/398px-Sandbox_with_interactive_projection_at_31c3.jpg) |

## Test 6

<img style="float: right;" src="https://upload.wikimedia.org/wikipedia/commons/2/2e/Sandbox_with_interactive_projection_at_31c3.jpg">

## Test 7

| - | - |
|---|---|
| Text left  | ![Flowers](https://upload.wikimedia.org/wikipedia/commons/2/2e/Sandbox_with_interactive_projection_at_31c3.jpg) |
| ![Flowers](https://upload.wikimedia.org/wikipedia/commons/2/2e/Sandbox_with_interactive_projection_at_31c3.jpg) | Text right |
