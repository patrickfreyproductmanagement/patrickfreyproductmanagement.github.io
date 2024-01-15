---
layout: page
title: People
permalink: /people/
---

There's a number of lean product management people that I follow, whose contributions I admire and where I take inspiration from their vast experience and wisdom. 

<div class="cards-3">
{% assign sorted_people = site.people | sort: 'order' %}
{% for person in sorted_people | sort: order %}    
    <div class="card">
        <a href="{{ person.url | relative_url }}">
            {% if person.image_url %}
                <img src="{{ person.image_url }}" alt="{{ person.name }}">
            {% else %}
                <img src="{{ '/assets/people/' | relative_url }}{{ person.image }}" alt="{{ person.name }}">
            {% endif %}           
        </a>        
    </div>
    <div class="card">        
        <strong>{{ person.name }}</strong>        
        <br/>
        <p>
          {{ person.summary }}
        </p>        
        <a href="{{ person.url | relative_url }}"><b>More</b></a>
    </div>    
{% endfor %}
</div>    