---
title: "Meet Our Team"
permalink: /team/
layout: single
---

# Meet the Tech Titans! 🧱

{% for member in site.data.team.members %}
## {{ member.name }}
- **Role:** {{ member.role }}
- **Age:** {{ member.age }}
- **Fun Fact:** {{ member.fun_fact }}
- **Hobbies:** {{ member.hobbies | join: ", " }}

---
{% endfor %}

## Join Our Team!
Interested in robotics? Contact us to learn more about joining the Tech Titans!