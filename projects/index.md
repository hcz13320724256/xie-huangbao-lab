---
title: 科研项目
nav:
  order: 2
  tooltip: 科研项目与成果转化
---
# 科研项目

{% for project in site.data.lab.researchProjects %}
## {{ project.title }}

- **项目来源**：{{ project.source }}
- **项目编号**：{{ project.number }}
- **执行周期**：{{ project.period }}
- **承担角色**：{{ project.role }}
- **项目状态**：{{ project.status }}
{% if project.funding != empty %}- **项目经费**：{{ project.funding }}{% endif %}

{{ project.description }}
{% if project.url != empty %}[项目主页]({{ project.url }}){% endif %}

{% endfor %}

{% include section.html %}

# 项目成果

{% for project in site.data.lab.projects %}
## {{ project.title }}
### {{ project.subtitle }}

{{ project.description }}

{{ project.year }} · {{ project.status }}

{{ project.tags | join: " · " }}
{% if project.url != empty %}[项目主页]({{ project.url }}){% endif %}
{% endfor %}
