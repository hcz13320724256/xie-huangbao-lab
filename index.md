---
title: 首页
---
# 理解自我，连接他人

我们关注自我与社会认知如何在大脑、关系和情境中发生变化，并将机制研究转化为更可靠的心理评估与干预线索。

{% include button.html link="research/" text="浏览论文成果" icon="fa-solid fa-book-open" %}
{% include button.html link="team/" text="认识团队" icon="fa-solid fa-users" %}

{% include section.html %}

## 把人的经验放回大脑、关系与情境之中

蟹黄堡实验室以认知神经科学为基础，研究自我加工、社会认知、共情及精神分裂症相关机制。我们重视理论问题与可检验预测的衔接，也关注实验范式、脑电指标和计算模型如何服务真实世界中的心理评估。

> 好的研究既要解释一个效应为何出现，也要说明它在什么条件下不再成立。

{% include section.html %}

## 研究方向

{% for area in site.data.lab.researchAreas %}
### {{ area.title }} · {{ area.subtitle }}
{{ area.description }}

{{ area.keywords | join: " · " }}

{% endfor %}

{% include section.html %}

## 研究与转化

{% include button.html link="projects/" text="科研项目与项目成果" icon="fa-solid fa-flask" %}
{% include button.html link="contact/" text="加入我们 / 联系实验室" icon="fa-regular fa-envelope" %}

以严谨的方法理解自我、他人与社会世界。
