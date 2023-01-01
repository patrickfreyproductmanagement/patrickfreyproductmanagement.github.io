---
layout: page
title: Books
permalink: /books/
---

Over the past years, product management has changed significantly primarily due to the influence and successes of Silicon Valley tech companies. 

When I started my product management career in 2011, I was both lucky and not so lucky:

I was lucky that I did not have any prior product management experience and thus did not have to unlearn any old-fashioned patterns. Also, I was lucky that there were few inspirational leader5s who encoraged me to follow my own instincts and try out something new. 

On the other hand, I was not so lucky as there was hardly any professional training material available for succeeding with new products. Most of the material available inside the company was describing how to manage existing products as part of the product engineering process. While some of the material was relevant, none of it was state-of-the-art and tailored for software products. 

I was this when I realized that most knowledge can be acquired through self-study, primarily through reading online articles or books written by innovators, great product leaders and others. 

<ul>
{% for book in site.books %}
  <li>
    <a href="{{ book.url }}"><b>{{ book.author }}:</b> {{ book.title }}</a>
  </li>
{% endfor %}
</ul>

<br/>
<hr/>
<br/>

## The CUBUDE method

[CUBUDE](/cubude) is a method I have developed for prioritizing product backlogs. 

{% include cubude_downloads.markdown %}
