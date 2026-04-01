---
id: "teaching"
title: "Blogs"
short: "Blogs"
icon: fa-book
sort_by_number: 6 
---
<div class="w3-row-padding">
{% for item in site.data.blogs %}    
      <div class="w3-half projects">
        <ul class="w3-ul w3-white w3-center w3-opacity w3-hover-opacity-off">
          <li class="w3-blue w3-large">{{item.title}}</li>
          <li class="w3-padding-16 w3-justify">{{item.url}}</li>
          <li class="w3-gray w3-justify">{{item.url}} </li>
        </ul>
      </div>
{% endfor %}
</div>

