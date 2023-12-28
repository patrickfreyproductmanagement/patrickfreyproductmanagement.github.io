---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

<h1>Hi,</h1>
<div class="cards">
    <div class="card">
        <p>
        I'm <b><a href="{{ '/about' | relative_url }}">Patrick</a></b>, a <b>passionate product manager</b> with over 15 years' experience in building software tools for automotive software engineers. 
        </p>
        <p>
            My <b>key interests</b> as product manager are 
            <ul>
                <li>
                    <b>building software-based products</b> that users <b>really like using</b>
                </li>
                <li>
                    <b>linking the customer value</b> delivered by the products (or services) <b>to prices and sales argumentations</b> that <b>convince customers</b> to invest and purchase, ultimately resulting in <b>profitable businesses</b>
                </li>
            </ul>
        </p>
    </div>
    <div class="card">
        <img class="profilepicture" src="{{ '/assets/Patrick_Frey_square_640x564_transparent_background.png' | relative_url }}" alt="Patrick Frey">
    </div>
</div>

On this site, I share [my experiences, personal views]({{ '/blog' | relative_url }}) as well as [methods and tools that I have adopted or developed]({{ '/custom_methods_and_tools' | relative_url }}). 


<h2>Check out my latest <a href="./blog">blog</a> posts</h2>
<ul>
  {% for post in site.posts limit:3 %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <span class="post-date">{{ post.date | date: "%B %-d, %Y" }}</span>
    </li>
  {% endfor %}
</ul>

<h2>Methods & Tools</h2>

Over the past 15 years, I have **tried out** a lot of methods, **adopted many** of them and even **developed** a set of **own methods and supporting tools** that have helped me to create a **successful new B2B business** at an existing large corporation. 

As the methods and tools have served me well, I want to share them to help others increasing their odds to succeed. 

{% include cube_teaser.html %}

{% include value_based_pricing_teaser.html %}

## Interested? Get in touch

If you're interested in lean product management in general or topics such as prioritization and value-based pricing, don't hesitate to get in touch ({% include get_in_touch.html %})!

There's a lot of material that I have developed to teach the methods as well as tools to apply them. 