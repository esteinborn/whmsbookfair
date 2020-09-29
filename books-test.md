---
layout: page
title: Book Test
permalink: /books-test/
---

{% assign booklist = site.data.books | sort: 'title'  %}

<h2 class="display-2">Primary Books</h2>
<div class="row row-cols-1 row-cols-md-4">
{% for book in booklist %}
  {% if book.age contains "P" %}
  <div class="col mb-5">
    <div class="card border-secondary shadow-sm h-100">
      <img src="{{ book.image }}" class="card-img-top" alt="{{ book.title }}">
      <div class="card-body">
        <h5 class="card-title">{{ book.title }}</h5>
        <p class="card-text">{{ book.author }}</p>
        <a href="{{ book.link }}" class="stretched-link">${{ book.price }}</a>
      </div>
    </div>
  </div>
  {% endif %}
{% endfor %}
</div>

<h2 class="display-2">Lower El</h2>
<div class="row row-cols-1 row-cols-md-4">
{% for book in booklist %}
  {% if book.age contains "LE" %}
  <div class="col mb-5">
    <div class="card border-secondary shadow-sm h-100">
      <img src="{{ book.image }}" class="card-img-top" alt="{{ book.title }}">
      <div class="card-body">
        <h5 class="card-title">{{ book.title }}</h5>
        <p class="card-text">{{ book.author }}</p>
        <a href="{{ book.link }}" class="stretched-link">${{ book.price }}</a>
      </div>
    </div>
  </div>
  {% endif %}
{% endfor %}
</div>
