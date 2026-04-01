---
id: "publications"
title:  "Publications"
short: "Publications"
icon: fa-file
sort_by_number: 4 
---
{% for item in site.data.publications %}  
- {{item.authors}} [{{item.title}}]({{item.url}}){{item.notes}}
{% endfor %}