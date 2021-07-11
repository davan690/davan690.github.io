---
title: Invasive Species Modelling
layout: page
css: "/css/index.css"
permlink: /invasive-species-modelling.html
meta-title: "New Zealands moonshot"
meta-description: "The New Zealand government set a Apollo shot to make NZ free of mammalian predators by 2050."
bigimg:
  - "/img/big-imgs/background-image.jpg" : "Auckland Islands, NZ (2011)"
  - "/img/national-leaders-announce-pfnz2050.png" : "Press release (2016)"
published: false
---

<div class="list-filters">
  <a href="/general-statistics" class="list-filter">Statistics</a>
  <a href="/ecological-statistics" class="list-filter">Ecology</a>
  <a href="/invasive-species-research" class="list-filter">PhD</a>
  <a href="https://www.ssnhub.com/beech-publication-wr" class="list-filter">Draft manuscript v1</a>
</div>

There was lots of press focus at the time (e.g. How [NZ might make PFNZ happen](https://news.nationalgeographic.com/2016/07/new-zealand-invasives-islands-rats-kiwis-conservation/);[Enviroment guide](http://www.environmentguide.org.nz/issues/biodiversity/key-threats/invasive-species/); [NZ geographic PFNZ plan](https://www.wired.com/2016/07/new-zealand-plans-kill-non-human-invasive-mammals/)) and academic interest too (extended info coming but most of the journal articles reference Russell et. al 2015 paper [here](https://academic.oup.com/bioscience/article/65/5/520/323246))

![](./img/national-leaders-announce-pfnz2050-title.png)
[Media release in 2016 announcing New Zealands Predator Free 2050 “apollo” shot](https://www.stuff.co.nz/environment/82454116/government-sets-target-to-make-new-zealand-predatorfree-by-2050).

Although I am unsure if this is even a good idea I do know from parts of my PhD research that it will be essential that New Zealands previous research, knowledge and data will be pivotal to achieving such a goal. This research has been produced in a reproducible workflow for national-scale predator control programs.

With the continued development of my PhD work I hope to be able to connect community groups with the statistical models needed to gain the timely ecological knowledge needed to response to pest control at a national scale. I believe that this will be vital for a on-going national monitoring needed for a PFNZ by 2050.

## News

<div class="post"><ul>
{% for post in site.tags["beech"] %}
  <a href="{{ post.url }}">{{ post.title }}</a> ({{ post.date | date_to_string }})<br>
    {{ post.description }}
{% endfor %}
</ul></div>

## My notes

Please excuse any '404' errors as I am learning and working as I go. Using version control and git means that I am able to use other coders templates and test things out before committing.