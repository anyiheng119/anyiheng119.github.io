---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
header:
  og_image: "research/IMG0102_resize.PNG"
---

<!-- My research falls into two general areas: developing novel tools to improve the study of phenotypes in a high-throughput manner and studying the variation and temporal basis of adaptive traits. Advanced methods such as machine learning, distributed computing, container technology, and computer vision are used throughout my research agenda.
-->

<!-- 
## Work in Progress

Data-Driven Incentive Optimization: Designing Employee Bonuses Using Decision-Focused Causal 
Learning 

Measuring Analytics Impact: Learning from 296 Franz Edelman Award Finalists
-->

## Research Presentations
**Yiheng An**, Jia Li, Jeffrey D. Camm (2024). "Smart Incentive Compensation: Designing Employee Bonuses Using Machine Learning and Analytics" Talk given at *School of Business, Wake Forest University* in Winston Salem, NC.

## Work in Progress

### Smart Incentive Compensation: Designing Employee Bonuses Using Machine Learning and Analytics

**Yiheng An**, <a href="https://business.wfu.edu/directory/jia-li/" target="_blank">Jia Li</a>(Wake Forest University), <a href="https://business.wfu.edu/directory/jeff-camm/" target="_blank">Jeffrey D. Camm</a>(Wake Forest University)

***Abstract*** Employee incentive compensation design, such as bonuses and commissions, is among the most important business decisions. However, traditional incentive plans often rely on static, predefined criteria, lacking customization and potentially leading to suboptimal business outcomes. In this study, we design a “smart” data-driven bonus system that uses machine learning (ML) and analytics to distribute targeted bonuses in real-time under budget constraints within a dynamic service environment. By integrating causal ML, predictive analytics, and prescriptive analytics, our system provides near-optimal bonus recommendations that account for critical contextual factors and service uncertainties.

The empirical application is developed in partnership with a Fortune Global 100 company. The objective is to enhance customer satisfaction within its customer service center by offering bonuses to customer support agents who manage more challenging cases. To begin, we conduct a large-scale field experiment (n=382,604) to evaluate the real-world effectiveness of bonuses in the service context. Next, we use causal ML methods to estimate the counterfactual effects of bonus decisions on customer satisfaction, conditional on key contextual factors such as customer characteristics (e.g., expected lifetime value), agent attributes (e.g., sensitivity to bonuses), case difficulty, and agent workloads. These estimates then serve as labels to train a supervised ML model that predicts the expected impact of bonuses on satisfaction. Finally, these predictions are treated as unknown parameters in a downstream optimization model that suggests bonus decisions.

Off-policy evaluation indicates that our solution can increase customer satisfaction rates for challenging cases by approximately 6.9% compared to a rule-based benchmark, yielding an estimated annual cost reduction of US$6.8 million. The technical advantage of our approach comes from three main aspects: (1) it leverages high-dimensional and dynamic data to capture service dynamics, enabling tailored, context-specific decisions; (2) by incorporating counterfactual predictions, it adapts to settings where certain decision parameters are unobservable; and (3) it accommodates any type of ML predictor, allowing flexible implementation based on the actual data quality and availability. Although our current empirical application focuses on customer service center bonuses, the proposed framework can be extended to a wide range of industries and incentive compensation designs.


<!-- 
<nbsp>

{% include base_path %}

{% assign ordered_pages = site.research | sort:"order_number" %}

{% for post in ordered_pages %}
  {% include archive-single.html type="grid" %}
{% endfor %}

-->