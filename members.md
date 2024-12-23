---
layout: page
title: Our Members

members:
  - name: Hansini Wadan
    img: /assets/members/hansi.webp
    role: Music Director
    instagram: https://instagram.com/hansini_wadan

  - name: Keshav Muralidharan
    img:  /assets/members/keshav.webp
    role: Assistant Music Director
    instagram: https://instagram.com/keshavmuralidharan

  - name: Luke Currier
    img:  /assets/members/luke.webp
    role: President
    instagram: https://instagram.com/currier_luke

  - name: Nevaeh Adu
    img:  /assets/members/vaeh.webp
    role: Brand Manager
    instagram: https://instagram.com/nevaeh.mo

  - name: Sam Brown
    img:  /assets/members/sam.webp
    role: Treasurer
    instagram: https://instagram.com/____sambrown____
    
  - name: Audrey Nguyen
    img:  /assets/members/audrey.webp
    role: 
    instagram: https://instagram.com/audreywguyen

  - name: Daniel Hellriegel
    img:  /assets/members/daniel.webp
    role: 
    instagram: https://instagram.com/danhellrie

  - name: Utsavi James
    img:  /assets/members/utsie.webp
    role: 
    instagram: https://instagram.com/utsavi_james

  - name: Jane Kaefer
    img:  /assets/members/jane.webp
    role: 
    instagram: https://instagram.com/janekaefer_

  - name: Izzy Pregiato
    img:  /assets/members/izzy.webp
    role: 
    instagram: https://instagram.com/iz.pregiato

  - name: Sky Martin
    img:  /assets/members/sky.webp
    role: 
    instagram: https://instagram.com/imskymartin

  - name: Joe Odetayo
    img:  /assets/members/joe.webp
    role: 
    instagram: https://instagram.com/jqsxph
---
<style>
  .members-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 50px;
  }

  .member-card {
    text-align: center;
    width: 200px; 
  }

  .member-card img {
    width: 200px;
    height: 200px;
    border-radius: 50%; 
    object-fit: cover;
    border: 3px solid #444; 
  }

  .title {
    font-size: 0.9em;
    color: #aaa;
  }

  @media (max-width: 768px) {
    .member-card {
      width: 120px;
    }
    .member-card img {
      width: 100px;
      height: 100px;
    }
  }
</style>

<div class="members-container">
  {% for member in page.members %}
  <div class="member-card">
    <a href="{{ member.instagram }}" target="_blank"><img src="{{ member.img }}" loading="lazy" alt="{{ member.name }}"></a>
    {% if member.instagram %}
      <a href="{{ member.instagram }}" target="_blank">{{ member.name }}</a>
    {% else %}
      <p>{{ member.name }}</p>
    {% endif %}
    {% if member.role %}
      <div class="title">{{ member.role }}</div>
    {% endif %}
  </div>
  {% endfor %}
</div>
