---
layout: page
title: Books
permalink: /books/
---

Over the past years, product management has changed significantly primarily due to the influence and successes of Silicon Valley tech companies. 

When I started my product management career in 2011, I was both lucky and not so lucky:

- I was lucky that I did not have any prior product management experience and thus did not have to unlearn any old-fashioned patterns. Also, I was lucky that there were few inspirational leaders who encouraged me to follow my own passion and try out something new. 

- On the other hand, I was not so lucky as there was hardly any professional training material available inside the company for succeeding with new products. Most of the material available was describing how to manage existing products as part of the product engineering process. While some of the material was relevant, none of it was state-of-the-art and tailored for agile software development projects. 

It was this when I realized that most knowledge can be acquired through self-study, primarily through reading online articles or books written by innovators, great product leaders and others. 

<!--
<ul>
{% for book in site.books %}
  <li>
    <a href="{{ book.url }}"><b>{{ book.author }}:</b> {{ book.title }}</a>
  </li>
{% endfor %}
</ul>
-->

The following list of books has helped and inspired me on my path to becoming a passionate product manager.

<div class="cards-3">
{% assign sorted_books = site.books | sort: 'order' %}
{% for book in sorted_books | sort: order %}    
    <div class="card">
        <a href="{{ book.url | relative_url }}">
            <img src="{{ '/assets/books/' | relative_url }}{{ book.cover_image }}" alt="{{ book.author }}:</b> {{ book.title }}">
        </a>        
    </div>
    <div class="card">
        {{ book.author }}
        <br/>
        <strong>{{ book.title}} </strong>        
        <br/>
        <br/>
        <p>
          {{ book.summary }}
        </p>        
        <a href="{{ book.url | relative_url }}"><b>More</b></a>
    </div>    
{% endfor %}
</div>    



<br/>
<hr/>
<br/>

{% include cube_teaser.html %}

{% include value_based_pricing_teaser.html %}


<!--
## The CUBE method

[CUBE](/CUBE) is a method I have developed for prioritizing product backlogs. 

{% include cube_downloads.markdown %}

-->
