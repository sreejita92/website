# IEEE@IIT Website

This is the website for the IEEE Illinois Institute of Technology student branch. The website is live at [ieeeiit.me](http://ieeeiit.me/).

## Tools used

* [Jekyll](http://jekyllrb.com/), a static site generator
* [Solid](https://st4ple.github.io/solid-jekyll/), a Bootstrap theme for Jekyll
* [Liquid](https://github.com/Shopify/liquid/wiki/Liquid-for-Designers), a template engine which was written with very specific requirements

---

This is a [Jekyll](http://jekyllrb.com/) port of the [Solid theme](http://www.blacktie.co/2014/05/solid-multipurpose-theme/) by [blacktie.co](http://www.blacktie.co/). Visit the [live demo](https://st4ple.github.io/solid-jekyll/) for a preview. 


##Usage
####Customize  
Most general settings and data like site name, colors, address, etc. can be configured and changed right in the main config file: `/_config.yml`
The content of the Home page can be changed here: `/home.html`
The content of the About page can be changed here: `/about.html`
The content of the Portfolio page can be changed here:`/portfolio.html`
The content of the Contact page can be changed here:`/contact.html`
####Add content  
Delete the demo content and publish your own content.
#####Blog post
Create a Blog post by creating a file called `yyyy-mm-dd-name-of-post-like-this.markdown` in the `/_posts/blog/` directory with the following template:
```markdown
---
layout: post          #important: don't change this
title: "Name of post like this"
date: yyyy-mm-dd hh:mm:ss
author: Name
categories:
- blog                #important: leave this here
- category1
- category2
- ...
img: post01.jpg       #place image (850x450) with this name in /assets/img/blog/
thumb: thumb01.jpg    #place thumbnail (70x70) with this name in /assets/img/blog/thumbs/
---
This text will appear in the excerpt "post preview" on the Blog page that lists all the posts.
<!--more-->
This text will not be shown in the excerpt because it is after the excerpt separator.
```
#####Project post
Create a Project post to go in your Portfolio by creating a file called `yyyy-mm-dd-name-of-the-project.markdown` in the `/_posts/project/` directory with the following template:
```markdown
---
layout: project       #important: don't change this
title:  "Name of the project"
date: yyyy-mm-dd hh:mm:ss
author: Name
categories:
- project             #important: leave this here
img: portfolio_10.jpg #place image (600x450) with this name in /assets/img/project/
thumb: thumb02.jpg
carousel:
- single01.jpg        #place image (1280x600) with this name in /assets/img/project/carousel/
- single02.jpg  
- ...
client: Company XY
website: http://www.internet.com
---
####This is a heading
This is a regular paragraph. Write as much as you like.
```
#####Question entry
Create a Question entry (that is listed in the Frequently Asked section on the Home page) in this directory by creating a file called `yyyy-mm-dd-do-i-have-a-question.markdown` in the `/_posts/project/` directory with the following template:
```markdown
---
layout: question
title:  "Do I have a question?"
date: yyyy-mm-dd hh:mm:ss
author: First Last
categories:
- question            #important: leave this here
---
####Can I use this theme for my website?
Of course you can!
```
####Publish
To publish with [GitHub Pages](https://pages.github.com/), simply create a branch called `gh-pages`in your repository. GitHub will build your site automatically and publish it at `http://yourusername.github.io/repositoryname/`.  
If there are problems with loading assets like CSS files and images, make sure that the `baseurl` in the `_config.yml`is set correctly (it should say `/repositoryname`).

##Site Map
```
. website
├── _includes
│   ├── css
│       ├── style.css
│   ├── carousel.html
│   ├── constitutionbylaws.html
│   ├── footer.html
│   ├── head.html
│   ├── header.html
│   ├── js.html
│   ├── members.html
│   ├── nav.html
│   ├── portfolio.html
│   ├── sidebar.html
│   ├── sponsors.html
│   ├── testimonial.html
│   ├── wrap.html
├── _layouts
│   ├── about.html
│   ├── contact.html
│   ├── default.html
│   ├── index.html
│   ├── newsletter.html
│   ├── portfolio.html
│   ├── post.html
│   ├── project.html
│   ├── style.css
├── _posts
│   ├── blog
│       ├── (all posts)
│   ├── project
│       ├── (all project descriptions)
│   ├── question (for FAQ section, currently invisible)
│       ├── (all questions)
├── assets
│   ├── css
│       ├── images (for layout)
│   ├── fonts
│   ├── img
│       ├── blog
│       ├── members (executive board only)
│       ├── project
│       ├── sponsors
│   ├── js
├── .gitignore
├── CNAME
├── README.md
├── _config.yml
├── about.html
├── category.html
├── contact.html
├── feed.xml
├── index.html
├── newsletter.html
├── project.html

```
