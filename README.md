# citygmlgurus.github.io

Source code for the website [citygml.guru](http://www.citygml.guru).
[Jekyll](http://www.jekyllrb.com) is used to generate static pages, and these are generated *automatically* after someone pushes to the repository (it may take ~30s to refresh though).

## Open datasets

Add the new CityGML open datasets should be added to `_data/opendatasets.yml`, it's a YAML (.yml) file and very simple to understand. 

The non-CityGML datasets (eg in COLLADA) should go to the file `_data/opendatasets_notcitygml.yml`


## Software

File is `_data/software.yml`, and the `category` field can contain more than one, eg:
```
- name: FME
  webpage: http://www.safe.com
  description: Can be used to read, write, process and visualise CityGML. macOS too now!
  foss: false
  category: viewer;parser
  starred: true
```

## Adding blog/news posts

Each blog/news post is a [Markdown](http://daringfireball.net/projects/markdown/syntax) file in `_posts`. 
When creating one, just copy the structure of the other ones, the naming convention for the files must be followed and each file should have a header of this form:

```
---
layout: post
title:  "Testing..1..2..testing"
categories: news
date:   2015-09-29 08:29
author: John Smith
---
```

To write markdown and see right-away the result, use that very handy [website](http://dillinger.io). 

To add images, you must them in the folder `/img/2016/myimg.jpg` and then add them with 

```
Bla bla bla 

![]({{ site.baseurl }}/img/2015/myimg.jpg)
```
