---
layout: default
---

<div class="home">

 <h1 class="page-heading">Blog</h1>

 {% for post in site.posts %}

    <div class="post">

   <h2>

​        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>

   </h2>

      <p class="post-meta">{{ post.date | date: "%B %-d, %Y" }}</p>

      <div class="post-excerpt">

​    {{ post.excerpt }}

   </div>

      <p><a href="{{ post.url | relative_url }}">Read more →</a></p>

  </div>

 {% endfor %}

</div>
