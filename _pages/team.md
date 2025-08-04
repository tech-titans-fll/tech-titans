---
title: "Meet Our Team"
permalink: /team/
layout: single
---

# Meet the Tech Titans! 🧱

**{{ site.team.full_name }}**  
*{{ site.team.school }} • {{ site.team.location }}*

---

## Our Team Members

{% for member in site.data.team.members %}
<div style="border: 2px solid #ff6b35; border-radius: 15px; padding: 20px; margin: 20px 0; background: #f8f9fa;">
  
  <div style="display: flex; align-items: center; gap: 20px; flex-wrap: wrap;">
    {% if member.photo %}
    <img src="{{ member.photo }}" alt="{{ member.name }}" style="width: 100px; height: 100px; border-radius: 50%; border: 3px solid #ff6b35; object-fit: cover;">
    {% else %}
    <div style="width: 100px; height: 100px; border-radius: 50%; background: linear-gradient(135deg, #ff6b35, #f7931e); display: flex; align-items: center; justify-content: center; color: white; font-size: 2rem; font-weight: bold;">
      {{ member.name | slice: 0 }}
    </div>
    {% endif %}
    
    <div style="flex: 1;">
      <h3 style="color: #007acc; margin-bottom: 5px;">{{ member.name }}</h3>
      <p><strong>{{ member.role }}</strong> • {{ member.grade }}</p>
      
      {% if member.description %}
      <p style="color: #555; margin: 10px 0;">{{ member.description }}</p>
      {% else %}
      <p style="color: #999; font-style: italic;">{{ member.name }}, add your description by editing _data/team.yml!</p>
      {% endif %}
      
      {% if member.fun_fact %}
      <p style="background: #e8f4fd; padding: 10px; border-radius: 8px; border-left: 4px solid #007acc;">
        💡 <strong>Fun Fact:</strong> {{ member.fun_fact }}
      </p>
      {% endif %}
    </div>
  </div>
</div>
{% endfor %}

---

## Our Mentors

{% for mentor in site.data.team.mentors %}
<div style="border: 2px solid #007acc; border-radius: 15px; padding: 20px; margin: 20px 0; background: #f0f8ff;">
  
  <div style="display: flex; align-items: center; gap: 20px; flex-wrap: wrap;">
    {% if mentor.photo %}
    <img src="{{ mentor.photo }}" alt="{{ mentor.name }}" style="width: 120px; height: 120px; border-radius: 50%; border: 3px solid #007acc; object-fit: cover;">
    {% else %}
    <div style="width: 120px; height: 120px; border-radius: 50%; background: linear-gradient(135deg, #007acc, #00a8ff); display: flex; align-items: center; justify-content: center; color: white; font-size: 2rem; font-weight: bold;">
      {{ mentor.name | slice: 0 }}
    </div>
    {% endif %}
    
    <div style="flex: 1;">
      <h3 style="color: #007acc; margin-bottom: 5px;">{{ mentor.name }}</h3>
      <p><strong>{{ mentor.role }}</strong></p>
      {% if mentor.organization %}<p>{{ mentor.organization }}</p>{% endif %}
      
      {% if mentor.description %}
      <p style="color: #555; margin: 10px 0;">{{ mentor.description }}</p>
      {% else %}
      <p style="color: #999; font-style: italic;"> {{ mentor.name }}, add your bio by editing _data/team.yml!</p>
      {% endif %}
      
      {% if mentor.link %}
      <p><a href="{{ mentor.link }}" style="color: #ff6b35; font-weight: bold;">Learn More →</a></p>
      {% endif %}
    </div>
  </div>
</div>
{% endfor %}

---

## How to Add Your Info

**Team members and mentors:** You can easily add your photo and description!

1. **Go to GitHub:** [Edit team.yml](https://github.com/tech-titans-fll/tech-titans/edit/main/_data/team.yml)
2. **Add your photo:** Upload to `/assets/images/team/` or `/assets/images/mentors/`
3. **Update your description:** Replace the placeholder text with your info
4. **Commit changes:** Your updates will appear on the website automatically!