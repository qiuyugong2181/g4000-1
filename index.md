---
layout: default
---

This website is for instructional purposes.

## People
<table>
    <thead>
        <tr>
            <th>First Name</th>
            <th>Last Name</th>
            <th></th>
            <th></th>
        </tr>
    </thead>
    <tbody>
        {% for page in site.pages %}
        {% if page.layout == "people" %}
        <tr>
            <td>{{page.first_name}}</td>
            <td>{{page.last_name}}</td>
            <td><a href="{{page.url | relative_url}}">profile</a></td>
            <td><a href="https://github.com/{{page.github_username}}">github page</a></td>
        </tr>
        {% endif %}
        {% endfor %}
    </tbody>
</table>
