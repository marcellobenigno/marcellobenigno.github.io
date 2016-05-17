---
layout: page
title: Banco de Dados Geográficos
permalink: /bdg/
---

## Notas de aula da disciplina

<div class="posts">
  
    <article class="post">
      {% for post in site.categories.bdg %}
      	<a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a> <br>
      {% endfor %}
    </article>
  
</div>