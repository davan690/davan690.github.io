---
title: Embedding a google location
cover-img: /assets/img/method-graf.jpg
thumbnail-img: "https://github.com/davan690/davan690.github.io/blob/1fb6c67142d60d993d123fd818d73bc4dde07465/assets/img/home_image1.jpg"
tags:
  - Google
  - Website
published: true
---
Google has a huge wealth of location data it uses for good or bad. It is possible to access and use this data for both personal interest and for the better side of the equation. 

## Quick links

- RShiny tutorial from [RStudio here](https://shiny.rstudio.com/tutorial/)

- RStudio shiny server [information here](https://www.rstudio.com/products/shiny/)

- My [predator prey simulation]("https://ssnhub.shinyapps.io/predator_prey_simulation1/") here [https://ssnhub.shinyapps.io/predator_prey_simulation1/]["https://ssnhub.shinyapps.io/predator_prey_simulation1/"]

# Background `iframe`

Here is the beginning of what I hope will be a collection of R scripts and notes on how to deal with google location data in R. Mostly because I have found this hard and I hope by writing a bunch of blog posts about it I will become more accustom to working with this sort of data.

`iframe` is one of the easiest way to embed an interactive web application inside a html webpage. In short, put maps in your documents from other applications online such as the my-maps map I have created below:

<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d102728.53602889985!2d149.96889269268158!3d-36.42693204654719!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x6b3e721c18d3ea21%3A0x40609b4904406a0!2sBermagui%20NSW%202546!5e0!3m2!1sen!2sau!4v1625880170565!5m2!1sen!2sau" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy"></iframe>

### Shiny app uses `iframe` too

The same `iframe` code can be used for a shiny app hosted on the [rstudio shiny server](https://shinyapps.io/) (5 free apps as of June 2021). There is also a package to make uploading and publishing your shiny app much easier [here]("https://rstudio.github.io/rsconnect/") These resources are a great tool for accessing and communicating early development of `RShiny` apps over the web. 

```
<iframe 
	src=<"YOUR-SHINY-APP">
	width=<"MEASUREMENT"> 
    height=<"MEASUREMENT"> 
    style="border:0;" 
    allowfullscreen="" 
    loading="lazy">
 </iframe> # finish code
```

And then it can look something like this:

<iframe src="https://ssnhub.shinyapps.io/predator_prey_simulation1/" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy"></iframe>