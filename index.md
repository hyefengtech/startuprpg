---
layout: default
title: Home
active: home
---
<div class="hero">
  <p class="kicker">Solo VC</p>
  <h1>아이디어에 투자하고,<br>실험으로 증명합니다.</h1>
  <p class="sub">여러 서비스가 흩어진 MVP가 아니라, 하나의 포트폴리오입니다. 각 프로젝트는 문제/가설/임팩트를 가진 투자 실험으로 운영됩니다.</p>
  <div class="cta">
    <a class="button" href="{{ '/portfolio' | relative_url }}">포트폴리오 보기</a>
    <a class="button secondary" href="{{ '/blog' | relative_url }}">LP Letter 구독</a>
  </div>
</div>

<div class="section">
  <h2>대표 포트폴리오</h2>
  <div class="grid">
    {% for p in site.data.portfolio limit:3 %}
      <div class="card">
        <span class="badge">{{ p.stage }}</span>
        <h3>{{ p.name }}</h3>
        <p class="meta">{{ p.problem }}</p>
        <p>핵가치: {{ p.value }}</p>
        <div class="cta">
          {% if p.cta_url %}<a class="button" href="{{ p.cta_url }}" target="_blank" rel="noopener">{{ p.cta_label | default: "체험하기" }}</a>{% endif %}
        </div>
      </div>
    {% endfor %}
  </div>
</div>