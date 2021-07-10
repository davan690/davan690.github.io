---
published: false
---
## Observations from the ALA of koalas 

There are a collection of functions and packages I have been using recently to access the citizen science data repository of Koala observations (the amazing ALA).

There are many tools that access and use the data associated with the ALA. To find an updated list of them in all their glory see the ALA website [website here]().

In particular I have been using the spatial portal to visualise the data and then think about the best way to capture this information directly from the API (through a package like `galah` is great). There are some challenges with this workflow but I have managed to make it work for the first few pieces of work now and I hope it will get quicker.

## Quickest way

I have found that the `galah` package is very easy to capture and investigate particular sections of the database. Here are a few snippets of code that I have been using:

[rcode here]