---
title: "科研"
layout: textlay
excerpt: "Optimization Group -- Research"
sitemap: false
permalink: /research/
---

# 科研

团队是国内率先进行算法博弈和相关优化理论研究的团队之一。团队以合作博弈的算法与复杂性、次模优化、图结构与算法为研究主线。

#### 算法博弈(Algorithmic Game Theory)

**算法博弈**(**Algorithmic Game Theory**)又称计算机经济学(Economics and Computation)，属于数学与计算机科学、经济学的交叉学科，通过计算机科学的视角与工具对博弈论进行研究。在合作博弈方面，团队重点研究合作分配方案（如核心、核仁、Shapley值、PMAS等）的存在性与计算复杂性以及特征值函数的次模性。在非合作博弈方面，团队从机制设计角度对各种均衡的收敛性与计算复杂性、无政府代价（PoA）、稳定代价（PoS）等进行研究。

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>


#### 次模优化(Submodular Optimization)

**次模优化**(**Submodular Optimization**)是离散优化的重要分支，在经济学、计算机科学以及机器学习、人工智能等领域有重要应用背景。次模性作为凸性的离散版本，在离散优化中发挥着关键的作用，许多经典的组合优化问题都可归结为次模优化问题。团队主要研究目标函数为（非）次模函数的离散优化问题的计算复杂性与近似算法。此外，作为上述理论与方法的应用，团队还研究社交网络中的影响最大化问题、利润最大化问题、谣言阻断问题等。


{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>

#### 图结构与算法(Graph Structures and Algorithm)

**图结构与算法** 图论(Graph Theory)起源于著名的Königsberg七桥问题，在计算机科学、管理科学、数据科学、信息科学等众多领域中都有重要应用背景。团队一方面研究图结构的划分问题，如图的染色问题、k-核等；另一方面还重点从图结构的角度进行算法设计与计算复杂性分析，为其他领域存在组合结构的关键问题提供理论与算法支持。


