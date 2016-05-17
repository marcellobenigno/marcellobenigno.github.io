---
layout: page
title: Banco de Dados Geográficos
permalink: /bdg/
---

## Notas de aula da disciplina

<div class="posts">
  
    <article class="post">

      <ul>
      {% for post in site.categories.bdg %}
      <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
      {% endfor %}
      </ul>

    </article>
  
</div>