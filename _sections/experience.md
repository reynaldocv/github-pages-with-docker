---
id: "experience"
short: "Experience"
title:  "Experience"
icon: fa-briefcase
sort_by_number: 3 
---
{% for item in site.data.experiences %}  
- <table class="table-experience">
    <tr>
      <td> {{item.institution}} 
        (<a href="{{item.institution_url}}">{{item.institution_short}}</a>)
      </td>
      <td style='text-align:right'><sub>{{item.city}}</sub></td>
    </tr>
    <tr>
      <td class="w3-lightgray"><b>{{item.possition}} </b></td>      
      <td style='text-align:right'><sup>{{item.start}} - {{item.end}}</sup></td>
    </tr>
    <tr>      
      <td class="w3-lightgray" colspan='2'>
      {{item.description}}
      </td>
    </tr>   
  </table>     
{% endfor %}