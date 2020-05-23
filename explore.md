---
layout: main
header: TB Explo
---
## Explore the looser side of my portfolio
### main topics:
<div class="explore-container">
{% for item in site.data.explore-topics %}
    <div class="explore-topic">
        {{ item.name }}
    </div>
{% endfor %}
</div>