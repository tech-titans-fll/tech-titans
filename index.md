---
layout: home
author_profile: true
title: "Welcome to Tech Titans!"
excerpt: "First LEGO League Team from Eagle Ridge Middle School"
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/hero-bg.jpg
  actions:
    - label: "Meet Our Team"
      url: "/team/"
---

# Welcome to Tech Titans! 🧱🤖

**Tech Titans First LEGO League Team**  
*Eagle Ridge Middle School • Ashburn, Virginia*

We are 7 passionate 6th grade creators dedicated to:
- **Building awesome robots** 🤖
- **Solving real-world problems** 🌍  
- **Learning together as a team** 🤝
- **Having fun with STEM** 🚀

## About Our Team

The Tech Titans are a group of 7 dedicated students from Eagle Ridge Middle School in Ashburn, Virginia. We're excited to compete in the {{ site.team.season }} FIRST LEGO League season!

**Our Mentors:**
- **Venkatesh** - Lead Mentor (Robotics for Youth Virginia)
- **Shyam Bhagwat** - Co-Mentor

## Latest Updates

{% for post in site.posts limit:3 %}
<div style="border: 1px solid #ddd; padding: 20px; margin: 20px 0; border-radius: 10px;">
  <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
  <p><small>{{ post.date | date: "%B %d, %Y" }}</small></p>
  <p>{{ post.excerpt }}</p>
</div>
{% endfor %}

## Team Stats

<div style="display: flex; justify-content: center; gap: 40px; margin: 30px 0; flex-wrap: wrap;">
  <div style="text-align: center;">
    <div style="font-size: 2.5rem; font-weight: bold; color: #ff6b35;">7</div>
    <div>Team Members</div>
  </div>
  <div style="text-align: center;">
    <div style="font-size: 2.5rem; font-weight: bold; color: #007acc;">6th</div>
    <div>Grade Level</div>
  </div>
  <div style="text-align: center;">
    <div style="font-size: 2.5rem; font-weight: bold; color: #ff6b35;">{{ site.team.season }}</div>
    <div>Season</div>
  </div>
</div>

---

*Check back regularly for updates on our robot progress and competition results!*