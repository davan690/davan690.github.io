---
title: Embedding a google location
cover-img: /assets/img/method-graf.jpg
thumbnail-img: /assets/img/method-graf.jpg
share-img: /assets/img/method-graf.jpg
tags:
  - Google
  - Website
published: true
---
Google has a huge wealth of location data it uses for good or bad. It is possible to access and use this data for both personal interest and for the better side of the equation. Here is the beginning of what I hope will be a collection of information on how to deal with google location data in R. Mostly because I have found this hard and I hope by writing a bunch of blog posts about it I will become more accustom to working with this sort of data.

## `iframe`

`iframe` is one of the easiest way to embed an interactive web application inside a html webpage. In short, put maps in your documents from other applications online such as the my-maps map I have created below:

<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d102728.53602889985!2d149.96889269268158!3d-36.42693204654719!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x6b3e721c18d3ea21%3A0x40609b4904406a0!2sBermagui%20NSW%202546!5e0!3m2!1sen!2sau!4v1625880170565!5m2!1sen!2sau" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy"></iframe>

### Shiny app uses `iframe` too

The same `iframe` code can be used for a shiny app hosted on the rstudio shiny server (5 free apps as of June 2021). This is a great resource for accessing and communicating RShiny apps over the web.

```
<iframe 
	src="<YOUR SHINY APP>" 
	width="600" 
    height="450" 
    style="border:0;" 
    allowfullscreen="" 
    loading="lazy">
 </iframe> # finish code
```

And then it can look something like this:

<iframe src="https://cjbattey.shinyapps.io/driftR/" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy"></iframe>

