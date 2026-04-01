---
id: "projects"
title:  "Projects"
short:  "Projects"
icon: fa-copyright
sort_by_number: 5
---

{% for item in site.data.projects %}  
- <table class="table-experience">
    <tr>
      <td class="w3-lightgray">
      <b> {{item.title}}</b> <a target="_blank" href="{{item.url}}"><i class="fa fa-github"></i></a>
        
      </td>
      <td style='text-align:right;color:red'><sup>{{item.status}}</sup></td>
    </tr>
    <tr>
      <td colspan="2" class="w3-justify">{{item.description}}</td>
    </tr>
    <tr>
      <td colspan="2" class="w3-light-gray" >
      <sub> {{item.software}} </sub>
      </td>
    </tr>   
  </table>  
  {{item.footer}}
{% endfor %}