---
published: true
tags:
  - Beech
---

# Mapping national parks in the US

I found this great shiny app that I have managed to reproduce on my shiny server. The next step is to recreate it with some new or different data. Link [here](https://ssnhub.shinyapps.io/shinyMapping/).

## Similar github projects

</div>
  <div class="col-md-4 col-md-offset-0 col-sm-4 col-sm-offset-0 col-xs-12 col-xs-offset-0 text-center">
    <div class="project-card">
      {%- assign gh-project = "reproducible-guidebook" -%}
      <a target="_blank" href="https://github.com/{{- gh-user -}}/{{- gh-project -}}" class="project-link" title="Go to Github Poject Page">
        <span class="fa-stack fa-4x">
          <i class="fa fa-circle fa-stack-2x stack-color"></i>
          <i class="fa fa-file-code-o fa-stack-1x fa-inverse"></i>
        </span>
        <h4>{{- gh-project -}}</h4>
        <hr class="seperator">
        <p class="text-muted">Building on the British Ecological Society guidebook on reporducible code.</p>
        <hr class="seperator">
        <img src="https://img.shields.io/github/forks/{{- gh-user -}}/{{- gh-project -}}.svg?style=social&label=Fork" alt="Github" title="Github Forks">
        <img src="https://img.shields.io/github/stars/{{- gh-user -}}/{{- gh-project -}}.svg?style=social&label=Stars" alt="Github" title="Github Stars">
      </a>
    </div>
  </div>

## News

<div class="post"><ul>
{% for post in site.tags["beech"] %}
  <a href="{{ post.url }}">{{ post.title }}</a> ({{ post.date | date_to_string }})<br>
    {{ post.description }}
{% endfor %}
</ul></div>

## My notes

Please excuse any '404' errors as I am learning and working as I go. Using version control and git means that I am able to use other coders templates and test things out before committing.