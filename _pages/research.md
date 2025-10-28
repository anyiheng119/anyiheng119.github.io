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

## Conference Proceedings (Peer-reviewed)

"IMPACT: An Inference-Driven Modeling Framework for Cost-Effective Incentive Allocation in Service Operations," 2025. 
 **Yiheng An**, Jia Li, Jeffrey D. Camm, Liang Hu, Qinqin Zhuge, Bingxin Jia. The 3rd Workshop on Causal Inference and Machine Learning in Practice at the 31st ACM ***SIGKDD*** Conference on Knowledge Discovery and Data Mining.


## Research Presentations

"Integrated Intelligence in Action: Designing Personalized Real-Time Incentives for Customer Service Agents", ***Conference on Artificial Intelligence, Machine Learning, and Business Analytics*** in New York, NY. December, 2025.

"Personalized Real-Time Incentives for Customer Service Agents: An Intelligent Decision-Support System", ***Conference on Information Systems and Technology (CIST)*** in Atlanta, GA. October, 2025.

"IMPACT: An Inference-Driven Modeling Framework for Cost-Effective Incentive Allocation in Service Operations", the 3rd Workshop on Causal Inference and Machine Learning in Practice at the ***31st ACM SIGKDD Conference on Knowledge Discovery and Data Mining*** in Toronto, ON, Canada. August, 2025.

"Smart Incentive Compensation: Designing Employee Bonuses Using Machine Learning and Analytics", the ***Annual POMS Conference*** in Atlanta, GA. May, 2025.

"Smart Incentive Compensation: Designing Employee Bonuses Using Machine Learning and Analytics", ***Annual Meeting of Southeast Decision Sciences Institute (SEDSI)*** in Greenville, SC. January, 2025.

"Smart Incentive Compensation: Designing Employee Bonuses Using Machine Learning and Analytics", ***School of Business, Wake Forest University*** in Winston Salem, NC. November, 2024.


## Work in Progress

### Smart Incentive Compensation: Designing Employee Bonuses Using Machine Learning and Analytics

**Yiheng An**, <a href="https://business.wfu.edu/directory/jia-li/" target="_blank">Jia Li</a> (Wake Forest University), <a href="https://business.wfu.edu/directory/jeff-camm/" target="_blank">Jeffrey D. Camm</a> (Wake Forest University)

***Abstract*** Employee incentive compensation design, such as bonuses and commissions, is among the most important business decisions. However, traditional incentive plans often rely on static, pre-defined criteria, lacking customization and potentially leading to limited effectiveness. In this study, we design a “smart” data-driven bonus system that uses machine learning (ML) and analytics to proactively distribute targeted bonuses in real-time under budget constraints within a dynamic service environment. By integrating causal ML, predictive analytics, and prescriptive analytics, our system provides near-optimal bonus recommendations that account for critical contextual factors and service uncertainties.

The empirical application is developed in partnership with a Fortune Global 100 company in China. The objective is to enhance customer satisfaction within its customer service center by offering bonuses to customer support agents who manage more challenging cases. To begin, we conduct a large-scale field experiment (n=382,604) to evaluate the real-world effectiveness of bonuses in the service context. Next, we use causal ML methods to estimate the counterfactual effects of bonus decisions on customer satisfaction, conditional on key contextual factors such as customer characteristics (e.g., expected lifetime value), agent attributes (e.g., service quality, workloads), and case attributes (e.g., case difficulty). These estimates then serve as labels to train a supervised ML model that predicts the expected impact of bonuses on satisfaction. Finally, these predictions are treated as unknown parameters in a downstream optimization model that suggests bonus decisions.

Off-policy evaluation indicates that our solution can increase customer satisfaction rates for challenging cases by approximately 4.77% compared to a rule-based benchmark, yielding an estimated annual cost reduction of US$ 4.66 million. The technical advantage of our approach comes from three main aspects: (1) it leverages high-dimensional and dynamic data to capture service dynamics, enabling tailored, context-specific decisions; (2) by incorporating counterfactual predictions, it adapts to settings where certain decision parameters are unobservable; and (3) it accommodates any type of ML predictor, allowing flexible implementation based on the actual data quality and availability. Although our current empirical application focuses on customer service center bonuses, the proposed framework can be extended to a wide range of industries and incentive compensation designs.



<!-- 

<html>
  <head>
    <style>
      .container {
        display: flex;
        flex-wrap: wrap;
      }
      section {
        flex: 1;
      }
      iframe {
        width: 100%;
        height: 69vh;
      }
      @media (max-width: 600px) {
        .container {
          flex-direction: column;
        }
      }
    </style>
  </head>
  <body>
    <div class="container">
      <section>
        <h2>Presentation Slides</h2>
        <iframe src="https://drive.google.com/file/d/112mC2POncei1scYR5_Pv36q45KJZHQlk/preview" allow="autoplay"></iframe><br />
        <a href="https://drive.google.com/file/d/112mC2POncei1scYR5_Pv36q45KJZHQlk/view?usp=drive_link" target="_blank">Download</a><br />
      </section>
    </div>
  </body>
</html>

-->


<!-- 
<nbsp>

{% include base_path %}

{% assign ordered_pages = site.research | sort:"order_number" %}

{% for post in ordered_pages %}
  {% include archive-single.html type="grid" %}
{% endfor %}

-->