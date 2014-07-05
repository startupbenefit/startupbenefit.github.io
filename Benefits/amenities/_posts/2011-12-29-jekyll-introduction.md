---
layout: post
category: Play
tagline: "Supporting tagline"
tags : [intro, beginner, jekyll, tutorial]
services: zenbenefits.com
---

Lorem ipsum dolor sit amet, id eum eripuit minimum blandit, an copiosae facilisis vix, brute falli intellegam vix ne. An vis tacimates volutpat recteque, ut nonumes menandri sea. Reque cetero dissentias ei eos. Et vix minim consulatu hendrerit, ex ullum tation nam. Mel eleifend partiendo id, ei nec iudico quando. Modus invenire persequeris nec no, fugit iisque delicatissimi an vim, pri et elit deserunt forensibus.

Services
|favicon|name|description|link|

<table class="table table-hover table-condensed">
  {% for reccomendation in site.data.data %}
        <thead>
          <tr>
            <th class="col-sm-2"></th>
            <th class="col-sm-4"></th>
            <th class="col-sm-2"></th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>
              <a href="https://github.com/{{ reccomendation.github }}">
                {{ reccomendation.name }}
              </a>
            </td>
            <td>{{ reccomendation.stuff }}</td>
            <td>
              <ul>
                {% for item in reccomendation.items %}
                <li>{{item.part_no}}</li>
                {% endfor %}
              </ul>
            </td>
          </tr>
          </tbody>
  {% endfor %}
</table>

Articles
-Title/Link
-Author

<table class="table table-hover table-condensed">
  {% for reccomendation in site.data.data %}
        <thead>
          <tr>
            <th class="col-sm-2">Title</th>
            <th class="col-sm-4">Author</th>
            <th class="col-sm-2"></th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>
              <a href="https://github.com/{{ reccomendation.github }}">
                {{ reccomendation.name }}
              </a>
            </td>
            <td>{{ reccomendation.stuff }}</td>
            <td>
              <ul>
                {% for item in reccomendation.items %}
                <li>{{item.part_no}}</li>
                {% endfor %}
              </ul>
            </td>
          </tr>
          </tbody>
  {% endfor %}
</table>