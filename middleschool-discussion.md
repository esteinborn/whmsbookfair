---
layout: page
title: Middle School Book Discussion
permalink: /:path/middleschool-discussion.html
category: M
age: M
---

<div class="row">
  <div class="col">
  <img src="./images/header.jpg" class="rounded mx-auto d-block img-fluid" alt="Selection of Books as a decorative header">
    <div class="jumbotron bg-transparent">
      <h1 class="display-4">{{ page.title }}</h1>
      <hr class="my-4">
      <p class="lead">Welcome to our Discussion page for Middle School books. This is where our Book Fair chairs and librarian will be posting about the Middle School books, including the featured books listed in the right column of this page. We hope you join us, we're hoping the discussions can gather our community like the standard Book Fair has in the past.</p>
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
