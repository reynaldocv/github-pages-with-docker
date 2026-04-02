---
id: "education"
short: "Education"
title: "Education"
icon: fa-graduation-cap
sort_by_number: 1 
---

{% for item in site.data.educations %}  
- <table class="table-experience">
    <tr>
      <td> {{item.university}} 
        (<a href="{{item.university_url}}">{{item.university_short}}</a>)
      </td>
      <td style='text-align:right'><sub>{{item.city}}</sub></td>
    </tr>
    <tr>
      <td><b>{{item.degree}} </b></td>      
      <td style='text-align:right'><sup>{{item.start}} - {{item.end}}</sup></td>
    </tr>
    <tr>
      <td><b>{{item.thesis_label}}</b> <a href="{{item.thesis_url}}">{{item.thesis}}</a></td>      
      <td style='text-align:right'><sub><b>{{item.adviser_label}}</b> 
      <a href="{{item.adviser_url}}">{{item.adviser}}</a></sub></td>
    </tr>   
    <tr>
      <td colspan='2'>
      {% if item.seminaries_label %}
        <sub>        
        <a href="https:/{{ site.url }}/eng_course/.md">
        <i class="fa fa-file-o"> {{item.seminaries_label}} </i>
        </a>
        </sub>
      {% endif %}
      </td>
    </tr>  
  </table>     
  
{% endfor %}
