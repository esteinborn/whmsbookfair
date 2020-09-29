---
layout: page
title: Book Test
permalink: /books-test/
---

<ul>
    {% for book in site.data.books %}
      <li>
        <a href="{{ book.link }}">
          <img src="{{ book.image }}">
        </a>
      </li>
    {% endfor %}
    </ul>
