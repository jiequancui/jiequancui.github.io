---
layout: default
title: "Ph.D. Students"
permalink: /phd-students/
---

<h1>Ph.D. Students</h1>

<div class="student-row">
  {% assign phd_students = site.members | where: "category", "phd" %}
  {% for student in phd_students %}
    <div class="student-card">
      <img src="{{ student.image }}" alt="{{ student.name }}">
      <h3>{{ student.name }}</h3>
      <p>{{ student.description }}</p>
    </div>
  {% endfor %}
</div>

