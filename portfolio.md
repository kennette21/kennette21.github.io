---
layout: main
header: TBPortfolio
permalink: /
--- 
<h2>This is a list of Projects</h2>

{% for item in site.data.projects %}
[{{item.display-name}}]({% link projects/{{item.name}}.md %})
{% endfor %}
