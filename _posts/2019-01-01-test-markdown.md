---
layout: post
title: Markdown syntax
subtitle: Quick tips
tags:
  - markdown
  - tips
comments: true
published: true
---

This is a demo post from Dean's website to show you how to write blog posts with markdown.  I strongly encourage you to [take 5 minutes to learn how to write in markdown](https://markdowntutorial.com/) - it'll teach you how to transform regular text into `bold/italics/headings/tables/etc`.

## Simple syntax

**Here is some bold text**

## Here is a secondary heading
### Here is a third heading

Here's a useless table:

| Number | Next number | Previous number |
| :------ |:--- | :--- |
| Five | Six | Four |
| Ten | Eleven | Nine |
| Seven | Eight | Six |
| Two | Three | One |


Here's a code chunk:

~~~
var foo = function(x) {
  return(x + 5);
}
foo(3)
~~~

And here is the same code with syntax highlighting:

```javascript
var foo = function(x) {
  return(x + 5);
}
foo(3)
```

And here is the same code yet again but with line numbers:

{% highlight javascript linenos %}
var foo = function(x) {
  return(x + 5);
}
foo(3)
{% endhighlight %}

## Boxes
You can add notification, warning and error boxes like this:

### Notification

{: .box-note}
**Note:** This is a notification box.

### Warning

{: .box-warning}
**Warning:** This is a warning box.

### Error

{: .box-error}
**Error:** This is an error box.

### Working with images

> set following yaml variables: `layout: post`; `tags: <tagg_label>`

Images live in the `./assets/img/` folder following the same rules as the beautiful jekyll template. Overall jekyll uses liquid tags to and these usually found in the `assets` folder.

#### Classic markdown image syntax

How about a yummy crepe? Here are two sections of code for working with markdown syntax (code).

![Crepe: How about a yummy crepe?](https://s3-media3.fl.yelpcdn.com/bphoto/cQ1Yoa75m2yUFFbY2xwuqw/348s.jpg)

It can also be centered!

![Crepe: It can also be centered!](https://s3-media3.fl.yelpcdn.com/bphoto/cQ1Yoa75m2yUFFbY2xwuqw/348s.jpg){: .mx-auto.d-block :}