---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: seminaries
---

{% assign sorted_sections = site.sections | sort: "sort_by_number" %}
{% for section in sorted_sections %}    
<div class="w3-padding-32 w3-content w3-justify" id="{{section.id}}">
<h2 class="w3-text-black">{{section.title}}</h2>           
{{section.content}}     
</div>
{% endfor %}
