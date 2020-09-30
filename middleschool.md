---
layout: page
title: Middle School Books
permalink: /:path/middleschool.html
category: M
---

<div class="row">
  <div class="col">
    <div class="jumbotron bg-transparent">
      <h1 class="display-1">{{ page.title }}</h1>
      <!-- <p class="lead">This year we’re partnering with The Open Door Book Store to bring the Book Fair online!</p> -->
      <hr class="my-4">
      <p>Here are a selection of {{ page.title }} for students. [[INSERT MORE TEXT HERE]]</p>
    </div>
  </div>
</div>
<div class="row">
  <div class="col">
    <div class="card mb-5">
      <div class="row no-gutters">
        <div class="col-md-4">
          <a class="stretched-link" href="./middleschool-discussion.html"><img src="./images/discussion.jpg" class="card-img" alt="Group discussing different topics"></a>
        </div>
        <div class="col-md-8">
          <div class="card-body">
            <h5 class="card-title">Hop into our chat to ask questions and discuss age appropriate {{ page.title }}.</h5>
            <a class="stretched-link" href="./middleschool-discussion.html">Join the Discussion!</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

  {% include book-list.html %}
