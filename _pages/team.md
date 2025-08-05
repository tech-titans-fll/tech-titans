---
permalink: /team/
layout: single
author_profile: false
classes: wide
---

# Meet the Tech Titans! 🧱

**Tech Titans First LEGO League Team**  
*Eagle Ridge Middle School • Ashburn, Virginia*

---

## Our Team Members

{% for member in site.data.team.members %}
<div style="border: 2px solid #ff6b35; border-radius: 20px; padding: 25px; margin: 25px 0; background: linear-gradient(135deg, #ffffff, #f8f9fa); box-shadow: 0 5px 15px rgba(0,0,0,0.1); transition: transform 0.3s ease;">
  
  <div style="display: flex; align-items: center; gap: 25px; flex-wrap: wrap;">
    {% if member.photo %}
    <img src="{{ member.photo }}" alt="{{ member.name }}" style="width: 120px; height: 120px; border-radius: 50%; border: 4px solid #ff6b35; object-fit: cover; box-shadow: 0 4px 12px rgba(255, 107, 53, 0.3);">
    {% else %}
    <div style="width: 120px; height: 120px; border-radius: 50%; background: linear-gradient(135deg, #ff6b35, #f7931e); display: flex; align-items: center; justify-content: center; color: white; font-size: 2.5rem; font-weight: bold; box-shadow: 0 4px 12px rgba(255, 107, 53, 0.3);">
      {{ member.name | slice: 0 }}
    </div>
    {% endif %}
    
    <div style="flex: 1; min-width: 300px;">
      <h2 style="color: #007acc; margin-bottom: 8px; font-size: 1.8rem;">{{ member.name }}</h2>
      <p style="font-size: 1.1rem; color: #666; margin-bottom: 15px;"><strong>{{ member.role }}</strong> • {{ member.grade }}</p>
      
      {% if member.description %}
      <p style="color: #333; margin: 15px 0; font-size: 1rem; line-height: 1.6;">{{ member.description }}</p>
      {% else %}
      <div style="background: #f0f8ff; border: 1px solid #cce7ff; padding: 15px; border-radius: 10px; margin: 15px 0;">
        <p style="color: #007acc; margin: 0; font-style: italic;">
          {{ member.name }} will be adding their profile information soon! 🚀
        </p>
      </div>
      {% endif %}
      
      {% if member.fun_fact %}
      <div style="background: linear-gradient(135deg, #e3f2fd, #f0f8ff); padding: 15px; border-radius: 12px; border-left: 5px solid #007acc; margin-top: 15px;">
        <p style="margin: 0; color: #1565c0;">
          💡 <strong>Fun Fact:</strong> {{ member.fun_fact }}
        </p>
      </div>
      {% endif %}
    </div>
  </div>
</div>
{% endfor %}

---

<div style="text-align: center; background: linear-gradient(135deg, #f8f9fa, #e9ecef); padding: 40px; border-radius: 20px; margin: 40px 0;">
  <h2 style="color: #007acc; margin-bottom: 20px;">🎯 Ready to Build Amazing Robots!</h2>
  <p style="font-size: 1.1rem; color: #666; margin-bottom: 25px;">
    Our team of 7 dedicated students is excited to tackle the challenges of FIRST LEGO League!
  </p>
  <div style="display: flex; justify-content: center; gap: 30px; flex-wrap: wrap; margin-top: 25px;">
    <div style="text-align: center;">
      <div style="font-size: 2.5rem; color: #ff6b35; font-weight: bold;">7</div>
      <div style="color: #666;">Team Members</div>
    </div>
    <div style="text-align: center;">
      <div style="font-size: 2.5rem; color: #007acc; font-weight: bold;">6th</div>
      <div style="color: #666;">Grade Level</div>
    </div>
    <div style="text-align: center;">
      <div style="font-size: 2.5rem; color: #28a745; font-weight: bold;">1st</div>
      <div style="color: #666;">FLL Season</div>
    </div>
  </div>
</div>