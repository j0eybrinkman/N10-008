---
layout: default
---

{% for post in site.posts %}
  <h2><a href=" {{site.baseurl}}{{ post.url }} ">{{ post.title }}</a></h2>
  <p>{{ post.date | date_to_string }}</p>
{% endfor %}

<!-- 

mardown syntax for easy copy/paste

link
  [](){:target="_blank"}

image 
  [![]({{site.baseurl}}/img/)](){:target="_blank"}
  -->