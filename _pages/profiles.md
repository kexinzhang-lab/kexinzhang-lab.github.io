---
layout: page
permalink: /team/
title: team
description: The people behind our science.
nav: true
nav_order: 3
---

<div class="team-page">
  <section class="team-pi" id="kexin" aria-labelledby="kexin-name">
    <figure class="team-portrait">
      <img src="{{ '/assets/img/prof_pic.jpg' | relative_url }}" alt="Kexin Zhang" width="1254" height="1254" fetchpriority="high">
      <figcaption>
        {% for line in site.data.kexin.office %}{{ line | escape }}<br>{% endfor %}
        <a href="mailto:kexin.k.zhang@yale.edu">kexin.k.zhang@yale.edu</a>
      </figcaption>
    </figure>
    <div class="team-bio">
      <p class="team-role">Principal Investigator</p>
      <h2 id="kexin-name">Kexin Zhang, PhD</h2>
      <p class="team-appointment">Assistant Professor<br>Department of Molecular Biophysics &amp; Biochemistry<br>Yale University</p>
      <ul class="team-links" aria-label="About Kexin Zhang">
        <li><a href="{{ '/kexin/' | relative_url }}">Biography <span aria-hidden="true">&rarr;</span></a></li>
      </ul>
    </div>
  </section>

  <section class="team-members" aria-labelledby="graduate-students">
    <h2 id="graduate-students">Graduate students</h2>
    <ul class="team-member-list">
      <li>
        <h3>Hang Li</h3>
        <p>First-year PhD rotation student</p>
        <p class="team-member-program">BQBS · Yale University</p>
      </li>
    </ul>
  </section>

  <section class="team-members" aria-labelledby="undergraduate-students">
    <h2 id="undergraduate-students">Undergraduate students</h2>
    <ul class="team-member-list">
      <li class="team-member--with-photo" id="sam">
        <img class="team-member-photo" src="{{ '/assets/img/sam.jpg' | relative_url }}" alt="Samuel Wu" width="800" height="800" loading="lazy">
        <div>
          <h3>Samuel Wu</h3>
          <p class="team-member-program">Molecular Biophysics &amp; Biochemistry · Yale University</p>
          <p class="team-member-link"><a href="{{ '/team/sam/' | relative_url }}">Biography <span aria-hidden="true">&rarr;</span></a></p>
        </div>
      </li>
      <li class="team-member--with-photo" id="sekai">
        <img class="team-member-photo" src="{{ '/assets/img/sekai.jpg' | relative_url }}" alt="Sekai Griffiths-Ferguson" width="800" height="800" loading="lazy">
        <div>
          <h3>Sekai Griffiths-Ferguson</h3>
          <p class="team-member-program">Molecular Biophysics &amp; Biochemistry and Cognitive Science · Yale University</p>
          <p class="team-member-link"><a href="{{ '/team/sekai/' | relative_url }}">Biography <span aria-hidden="true">&rarr;</span></a></p>
        </div>
      </li>
    </ul>
  </section>

  <section class="team-join" aria-labelledby="join-team">
    <div>
      <p class="team-role">Grow with us</p>
      <h2 id="join-team">Join the team</h2>
    </div>
    <div>
      <p>We welcome postdocs, graduate students, master's students, and undergraduates interested in cryo-EM, AI, and computational structural biology. Projects can focus on methods, computation, or biological questions.</p>
      <p>Explore our <a href="{{ '/research/' | relative_url }}">research</a> and <a href="{{ '/' | relative_url }}#join-us--multiple-openings">current openings</a>, or <a href="mailto:kexin.k.zhang@yale.edu">email Kexin</a> with your CV and a short note about your interests.</p>
    </div>
  </section>
</div>
