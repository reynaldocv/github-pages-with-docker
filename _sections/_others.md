---
id: "experience"
short: "Others"
title:  "Others"
icon: fa-file
sort_by_number: 8 
---
{% for item in site.data.experiences %}  
- <table style="border:0px">
    <tr>
      <td> {{item.institution}} 
        (<a href="{{item.institution_url}}">{{item.institution_short}}</a>)
      </td>
      <td style='text-align:right'>{{item.city}}</td>
    </tr>
    <tr>
      <td><b>{{item.possition}} </b></td>      
      <td style='text-align:right'>{{item.start}} - {{item.end}}</td>
    </tr>
    <tr>      
      <td colspan='2'>
        - {{item.description}}
      </td>
    </tr>   
  </table>     
{% endfor %}