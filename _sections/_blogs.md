---
id: "blogs"
title: "Blogs"
short: "Blogs"
icon: fa-book
sort_by_number: 6 
---
<div class="w3-row-padding">
{% for item in site.data.blogs %}    
      <div class="w3-half">
         <ul class="w3-ul w3-pale-blue w3-center">
          <li class="w3-large blogs"><a href="{{item.url}}">{{item.title}}</a></li>         
        </ul>     
      </div>
      <hr>
{% endfor %}
</div>


