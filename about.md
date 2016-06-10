---
layout: page
title: About
permalink: /about/
order: 2
---

{% include about-the-course.html %}

Learn more about the course by visiting [http://bit.ly/polito-ami](http://bit.ly/polito-ami) or join the [Facebook group](https://www.facebook.com/groups/polito.ami). 

---

#### Teachers ####

<div class="mdl-grid" style="max-width: 800px;">
    
    {% for teacher in site.data.staff %}

    <div class="mdl-cell mdl-card mdl-cell--3-col-desktop" >
    
        <div class="mdl-card__media">
          <img class="card-image" src="{{teacher.image | prepend: site.baseurl }}" border="0" alt="{{teacher.name}}">
        </div>
        
        <div class="mdl-card__supporting-text">
           <p><strong>{{ teacher.name }}</strong><br/>
          {{ teacher.bio }}
          </p>
        </div>
    
    </div>
    
    <div class="mdl-cell mdl-cell--1-col-desktop mdl-cell--hide-tablet mdl-cell--hide-phone"><!-- intentionally left empty --></div>
    
    {% endfor %}

</div>