---
layout: single
title: "말해지지 않은 것들"
permalink: /
excerpt: "역사콘텐츠 플랫폼"
---

<p style="text-align:center">
  <a class="btn btn--primary btn--large" href="{{ '/history/' | relative_url }}">역사 아카이브 보기</a>
  <a class="btn btn--inverse btn--large" href="https://example.com/fandom" target="_blank" rel="noopener">연성 노트 보기</a>
  <a class="btn btn--large" href="{{ '/newsletter/' | relative_url }}">뉴스레터 보기</a>
</p>

## 타임머신은 없지만 기록으로 시대를 건넌다
역사와 서사를 사랑하는 기획자의 기록 공간  
자료를 모으고 해석하고 새로운 이야기의 씨앗으로 키웁니다

---

## 최신글 — 역사 아카이브
{% assign history_posts = site.history | sort: 'date' | reverse | slice: 0, 3 %}
<ul class="posts-list">
{% for doc in history_posts %}
  <li class="archive__item">
    <a href="{{ doc.url | relative_url }}" class="archive__item-title">{{ doc.title }}</a>
    <span class="page__meta">{{ doc.date | date: "%Y.%m.%d" }}</span>
    {% if doc.excerpt %}
      <p class="archive__item-excerpt">{{ doc.excerpt | strip_html | truncate: 120 }}</p>
    {% endif %}
  </li>
{% endfor %}
</ul>

## 연성 노트
<p>
  외부 사이트에서 연성 노트를 운영하고 있습니다.<br>
  아래 버튼을 눌러 이동하세요.
</p>
<p>
  <a class="btn btn--inverse btn--large" href="https://example.com/fandom" target="_blank" rel="noopener">
    연성 노트로 이동
  </a>
</p>

## 최신글 — 뉴스레터
{% assign nl_posts = site.newsletter | sort: 'date' | reverse | slice: 0, 3 %}
<ul class="posts-list">
{% for doc in nl_posts %}
  <li class="archive__item">
    <a href="{{ doc.url | relative_url }}" class="archive__item-title">{{ doc.title }}</a>
    <span class="page__meta">{{ doc.date | date: "%Y.%m.%d" }}</span>
    {% if doc.excerpt %}
      <p class="archive__item-excerpt">{{ doc.excerpt | strip_html | truncate: 120 }}</p>
    {% endif %}
  </li>
{% endfor %}
</ul>
