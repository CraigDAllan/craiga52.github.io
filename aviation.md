---
layout: default
---
<h1>Archive of aviation articles.</h1>

<ul>
{% for post in site.categories.aviation %}
    <article class="post">    
      
      <h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>

      <div class="entry">
        {{ post.content | truncatewords:40}}
      </div>
      
      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
    </article>
    {% endfor %}
</ul>
