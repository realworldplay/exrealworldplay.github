---
layout: single
title: "말해지지 않은 것들"
permalink: /
excerpt: "역사콘텐츠 플랫폼"
---

<!--
<p style="text-align:center">
  <a class="btn btn--primary btn--large" href="{{ '/history/'   | relative_url }}">역사 아카이브</a>
  <a class="btn btn--large" href="{{ '/xd/'        | relative_url }}">경험설계</a>
  <a class="btn btn--large" href="{{ '/columns/'   | relative_url }}">해설 칼럼</a>
  <a class="btn btn--large" href="{{ '/notes/'     | relative_url }}">연구 메모</a>
  <a class="btn btn--large" href="{{ '/fieldtrip/' | relative_url }}">현장 탐방</a>
  <a class="btn btn--large" href="{{ '/sources/'   | relative_url }}">사료 번역</a>
  <a class="btn btn--large" href="{{ '/curation/'  | relative_url }}">큐레이션</a>
  <a class="btn btn--inverse btn--large" href="https://realworldplay.github.io" target="_blank" rel="noopener">연성노트 보기</a>
  <a class="btn btn--large" href="https://maily.so/sayeon" target="_blank" rel="noopener">뉴스레터</a>
</p>
-->

## 타임머신은 없지만 기록으로 시대를 건넌다
역사와 서사를 사랑하는 기획자의 기록 공간  
자료를 모으고 해석하고 새로운 이야기의 씨앗으로 키웁니다

---

### 최신글 — 경험설계
{% assign posts = site.xd | sort: 'date' | reverse | slice: 0, 3 %}
<ul class="posts-list">
{% for doc in posts %}
<li class="archive__item">
  <a href="{{ doc.url | relative_url }}" class="archive__item-title">{{ doc.title }}</a>
  <span class="page__meta">{{ doc.date | date: "%Y.%m.%d" }}</span>
  {% if doc.excerpt %}<p class="archive__item-excerpt">{{ doc.excerpt | strip_html | truncate: 120 }}</p>{% endif %}
</li>
{% endfor %}
</ul>

### 최신글 — 해설 칼럼
{% assign posts = site.columns | sort: 'date' | reverse | slice: 0, 3 %}
<ul class="posts-list">
{% for doc in posts %}
<li class="archive__item">
  <a href="{{ doc.url | relative_url }}" class="archive__item-title">{{ doc.title }}</a>
  <span class="page__meta">{{ doc.date | date: "%Y.%m.%d" }}</span>
  {% if doc.excerpt %}<p class="archive__item-excerpt">{{ doc.excerpt | strip_html | truncate: 120 }}</p>{% endif %}
</li>
{% endfor %}
</ul>

### 최신글 — 연구 메모
{% assign posts = site.notes | sort: 'date' | reverse | slice: 0, 3 %}
<ul class="posts-list">
{% for doc in posts %}
<li class="archive__item">
  <a href="{{ doc.url | relative_url }}" class="archive__item-title">{{ doc.title }}</a>
  <span class="page__meta">{{ doc.date | date: "%Y.%m.%d" }}</span>
  {% if doc.excerpt %}<p class="archive__item-excerpt">{{ doc.excerpt | strip_html | truncate: 120 }}</p>{% endif %}
</li>
{% endfor %}
</ul>

### 최신글 — 현장 탐방
{% assign posts = site.fieldtrip | sort: 'date' | reverse | slice: 0, 3 %}
<ul class="posts-list">
{% for doc in posts %}
<li class="archive__item">
  <a href="{{ doc.url | relative_url }}" class="archive__item-title">{{ doc.title }}</a>
  <span class="page__meta">{{ doc.date | date: "%Y.%m.%d" }}</span>
  {% if doc.excerpt %}<p class="archive__item-excerpt">{{ doc.excerpt | strip_html | truncate: 120 }}</p>{% endif %}
</li>
{% endfor %}
</ul>

### 최신글 — 사료 번역
{% assign posts = site.sources | sort: 'date' | reverse | slice: 0, 3 %}
<ul class="posts-list">
{% for doc in posts %}
<li class="archive__item">
  <a href="{{ doc.url | relative_url }}" class="archive__item-title">{{ doc.title }}</a>
  <span class="page__meta">{{ doc.date | date: "%Y.%m.%d" }}</span>
  {% if doc.excerpt %}<p class="archive__item-excerpt">{{ doc.excerpt | strip_html | truncate: 120 }}</p>{% endif %}
</li>
{% endfor %}
</ul>

### 최신글 — 큐레이션
{% assign posts = site.curation | sort: 'date' | reverse | slice: 0, 3 %}
<ul class="posts-list">
{% for doc in posts %}
<li class="archive__item">
  <a href="{{ doc.url | relative_url }}" class="archive__item-title">{{ doc.title }}</a>
  <span class="page__meta">{{ doc.date | date: "%Y.%m.%d" }}</span>
  {% if doc.excerpt %}<p class="archive__item-excerpt">{{ doc.excerpt | strip_html | truncate: 120 }}</p>{% endif %}
</li>
{% endfor %}
</ul>

