---
title: "Choose Your Own Adventure"
description: "A Choose your own Adventure Website that was created using a static site generator"
categories: 
date: 2018-04-20
dropCap: false
displayInMenu: false
displayInList: true
draft: false
resources:
- name: featuredImage
  src: "Adventure-Mockup.png"
  params:
    description: "A screenshot of the Choose Your Own Adventure Website"
- name: featuredImageTall
  src: "Adventure-Mockup-tall.png"
  params:
    description: "A screenshot of the Choose Your Own Adventure Website"
- name: hierarchy
  src: "hierarchy.png"
  params:
    description: "A screenshot of the Choose Your Own Adventure Website"
---

### Project Brief

I was given a lof of freedom for this project, the goal was to design and build a website that makes use of a static site generator. The idea I developed was to create something fun that made use of how easily SSG's allow you to create mutiple pages because of their template system. So I decided to create a Choose your own adventure site, as these are very simple pages but there are a LOT of them. I really enjoyed the process and the fun of building something a little bit different. 

### Design
I knew I would only need three templates/layouts for the site, a 'home' page, a 'choice' page and a 'end' page. I drew up a hierarchy chart to create a flow for the game, so I knew exactly how many pages to build and which other pages they would link to.
The hierachry can be seen below:

{{<smallimg src="hierarchy" alt="A diagram that shows all the possible choice in the website" width="1000px">}}

### Creating the templates and pages
I created all three templats with tester pages first and made sure that each template was responsive. Once the templates had been created it was only a matter of creating the hierachy using them. This was done with a whole bunch of markdown files. The links were added to the yaml of each markdown file 

```yaml
---
# set the layout to use, in this case, a 'choice' page
layout: layouts/choice

# set the page title
title: Choose Your Own Adventure


# These are the links for choices
choice:
    link1: <a href='../left-1'>Left</a>
    link2: <a href='../right-1'>Right</a>
---

# The text which asks the user to make a decision
There is a fork in the cave. Do you go left or right?
```

### Try it Out
You can go take a look at the site [here](https://portfolio.clairelouisebutler.com/projects/adventure-website/live).

