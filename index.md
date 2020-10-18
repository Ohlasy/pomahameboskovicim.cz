---
layout: default
title: Pomáháme Boskovicím
description: Aktuální informace o koronaviru na Boskovicku, koordinace dobrovolnické pomoci
---

# Pomáháme Boskovicím

Celá společnost prochází koronavirovou pandemií a nemoc covid-19 se poměrně intenzivně šíří také v našem regionu – čísla nakažených rostou, boskovická nemocnice hlásí, že její kapacity se plní. Nyní je situace mnohem vážnější, než byla na jaře.

## Jak jsme na tom v regionu?

- Aktuální počty pozitivně testovaných k 17. říjnu:
  - Boskovice: nevíme
  - [ORP Boskovice](https://cs.wikipedia.org/wiki/Obvod_obce_s_rozš%C3%ADřenou_působnost%C3%AD_Boskovice): 478 (zhruba 1 % obyvatel)
  - okres Blansko: 978 (zhruba 1 % obyvatel)
- [Informace o stavu nemocnice](https://ohlasy.info/clanky/2020/10/situace-v-nemocnici.html) k 8. říjnu

## Co můžete dělat

V tuto chvíli je nejdůležitější chránit nejrizikovější skupiny obyvatel, především lidi starší a nemocné. Chránit je tím, že se všichni budeme chovat co nejzodpovědněji, omezíme maximálně svoje kontakty, budeme nosit ochranné pomůcky a dodržovat hygienická pravidla. A zároveň starší lidi přesvědčíme o tom, aby situaci brali vážně, aby se vyhýbali riziku.

## Zapojte se!

Pokud chcete pomáhat jako dobrovolník, klikněte na tlačítko níže a vyplňte formulář. Ozveme se vám, když bude potřeba.

<form action="https://bit.ly/pomahejbce">
    <input type="submit" value="Nabízím pomoc" />
</form>

## Informace z regionu

{% assign articles = site.array %}
{% for article in site.data.articles %}
{% if article.tags contains "koronavirus" %}
{% assign articles = articles | push: article %}
{% endif %}
{% endfor %}

<div class="articles">
{% for article in articles limit:6 %}
<a href="https://ohlasy.info{{ article.relativeURL }}" class="article-preview">
<img src="{{ article.cover-photo }}">
<p>{{ article.title}}</p>
</a>
{% endfor %}
</div>

## O webu

Na projektu spolupracují Farní sbor Českobratrské církve evangelické, Junák – český skaut, Ohlasy a Unijazz Boskovice.
Chcete nám s ním pomoct? Stačí se [přidat k nám do chatu](https://join.slack.com/t/koronabce/shared_invite/zt-ibg4iiw3-nB5d3B53aBkI_tcN0C1eqA)!

<pomahame@prostor.wtf>
