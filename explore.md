---
layout: main
header: TB Explo
---
## Explore the looser side of my portfolio
### main topics:
<div class="explore-container">
{% for item in site.data.explore-topics %}
    <div class="explore topic wobble-vertical-on-hover">
        <a href="explores/{{item.name}}.html">{{ item.name }}</a>
    </div>
{% endfor %}
</div>