---
layout: page
title: Lower Elementary Book Discussion
permalink: /:path/lowerel-discussion.html
category: LE
---

<div class="row">
  <div class="col">
    <div class="jumbotron bg-transparent">
      <h1 class="display-4">{{ page.title }}</h1>
      <!-- <p class="lead">This year we’re partnering with The Open Door Book Store to bring the Book Fair online!</p> -->
      <hr class="my-4">
      <p>Join our chat below to ask questions and discuss age appropriate {{ page.title }} for students. [[INSERT MORE TEXT HERE]]</p>
    </div>
  </div>
</div>
<div class="row">
  <div class="col-md-9">

  {% include disqus.html %}
                    
  </div>
  <div class="col-md-3 book-sidebar">
    
    {% include book-sidebar.html %}

  </div>
</div>

