---
layout: default
title: Weekly Blog 📝
---

# My Weekly Progress Reports ✍️

This section is dedicated to my weekly reflections and technical updates. By keeping these here, my Home page stays static and professional, while this blog section stays active and updated! ✨

---

{% for post in site.posts %}
<div style="border: 1px solid #ff69b4; padding: 20px; margin-bottom: 20px; border-radius: 12px; background: #111; box-shadow: 0 5px 15px rgba(255, 105, 180, 0.1);">
    <h2 style="margin-top: 0;">
        <a href="{{ post.url | relative_url }}" style="color: #ff69b4; text-decoration: none;">
            {{ post.title }}
        </a>
    </h2>
    <p style="font-size: 0.9rem; color: #888;">📅 Posted on: {{ post.date | date: "%B %d, %Y" }}</p>
    
    <a href="{{ post.url | relative_url }}" style="color: white; font-weight: bold; font-size: 0.8rem; text-transform: uppercase; text-decoration: none; border-bottom: 1px solid #ff69b4;">Read Reflection →</a>
</div>
{% endfor %}

{% if site.posts.size == 0 %}
<p>No posts yet! I'll be updating this very soon. Stay tuned! 🎀</p>
{% endif %}

---
