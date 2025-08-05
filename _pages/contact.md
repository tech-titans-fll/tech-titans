---
permalink: /contact/
layout: single
---

# Contact Tech Titans 📧

## Team Information

<div style="background: linear-gradient(135deg, #ff6b35, #f7931e); color: white; padding: 30px; border-radius: 15px; margin: 30px 0;">
  <h3 style="color: white; margin-bottom: 20px;">🧱 {{ site.team.full_name }}</h3>
  <p><strong>School:</strong> {{ site.team.school }}</p>
  <p><strong>Location:</strong> {{ site.team.location }}</p>
  <p><strong>Season:</strong> {{ site.team.season }}</p>
</div>

## Our Mentors

{% for mentor in site.data.team.mentors %}
<div style="border: 1px solid #ddd; padding: 20px; margin: 20px 0; border-radius: 10px;">
  <h4>{{ mentor.name }} - {{ mentor.role }}</h4>
  {% if mentor.organization %}<p><strong>{{ mentor.organization }}</strong></p>{% endif %}
  <p><em>Contact information will be added by mentors</em></p>
</div>
{% endfor %}

## Team Meetings

<div style="background: #f0f8ff; padding: 20px; border-radius: 10px; margin: 20px 0;">
  <h3 style="color: #007acc;">📍 Meeting Details</h3>
  <p><strong>Location:</strong> {{ site.team.meeting.location }}</p>
  <p><strong>Time:</strong> {{ site.team.meeting.time }}</p>
  <p><strong>Duration:</strong> 1 hour</p>
</div>

## About Our Meetings

Our team meets weekly to work on:
- **Robot Design & Building** - Hands-on construction with LEGO components
- **Programming** - Coding our robot to complete autonomous missions  
- **Research Project** - Investigating real-world problems and solutions
- **Core Values** - Practicing teamwork, discovery, and innovation
- **Competition Prep** - Getting ready for tournaments

## Questions?

If you have questions about our team or FIRST LEGO League, feel free to reach out to our mentors. We'd be happy to share more about our program!

---

<div style="text-align: center; padding: 30px; background: #f8f9fa; border-radius: 10px; margin: 30px 0;">
  <h3 style="color: #007acc;">Follow Our Journey!</h3>
  <p>Check back regularly for updates on our robot progress, competition results, and team activities.</p>
  <p style="font-size: 2rem;">🤖 🧱 🚀</p>
</div>