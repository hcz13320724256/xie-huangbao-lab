---
title: 论文成果
nav:
  order: 1
  tooltip: 检索实验室论文
---
# 论文成果

按题目、作者、期刊或年份检索。论文条目沿用实验室现有资料，作者贡献标注保留原有记录。

{% include search-box.html %}
{% include search-info.html %}

{% assign years = site.data.citations | group_by: "year" | sort: "name" | reverse %}
{% for year in years %}
## {{ year.name }}
{% for paper in year.items %}
{% include citation.html title=paper.title authors=paper.authors publisher=paper.publisher year=paper.year id=paper.id link=paper.link type=paper.type description=paper.description buttons=paper.buttons tags=paper.tags style="rich" %}
{% endfor %}
{% endfor %}
