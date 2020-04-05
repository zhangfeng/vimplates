---
title: Accueil
layout: default
---

## Bienvenue sur **vimplates.tk**

### Listes de **vimplates**

{% assign listes = site.pages | where:"layout", "plates" -%}
{% for l in listes -%}
- [{{ l.dir | replace:"/", ""}}]({{ l.url }})
{% endfor -%}
