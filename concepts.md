---
layout: page
title: Lean Product Gists
permalink: /concepts/
---

Short, easy to read and digest articles on key concepts of lean product management.

<h3>Product</h3>
<ol>
{% assign sorted_concepts = site.concepts | sort: 'order' %}  
{% for concept in sorted_concepts %}    
    <li>
        <a href="{{ concept.url }}">
            {{ concept.title }}
        </a>        
    </li>
{% endfor %}
</ol>

<h3>Methods</h3>
<ol>
{% assign sorted_methods = site.methods | sort: 'order' %}  
{% for method in sorted_methods %}    
    <li>
        <a href="{{ method.url }}">
            {{ method.title }}
        </a>        
    </li>
{% endfor %}
</ol>