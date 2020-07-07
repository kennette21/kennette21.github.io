---
layout: main
header: TB Explo
---
## Less professional, still me
<div class="explore-container">
    <div class="active-projects-list">
        {% for item in site.data.explore-topics %}
            {% unless item.hidden %}
                <a class="explore topic wobble-vertical-on-hover" href="explores/{{item.name}}.html">
                    {{ item.name }}
                </a>
                <div class="separator"></div>
            {% endunless %}
        {% endfor %}
    </div>
</div>