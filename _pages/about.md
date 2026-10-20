---
permalink: /
title: " "
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<p class="thesis-statement">I model how people disagree, then use that to personalize and align LLMs.</p>

Hi! I'm a fourth-year PhD student at the University of Michigan School of
Information (UMSI), advised by David Jurgens and part of the
[Blablablab](https://blablablab.si.umich.edu/). I work on NLP and
computational social science. Before Michigan, I received a BA in Statistics
and Data Science from UC Berkeley in 2023. In summer 2026 I was a research and development intern at Kitware, where I built **VISTA**, a system for steering LLMs using values inferred from a short survey.

My research is on <span class="accent-term">pluralistic alignment</span>: modeling how individuals
and groups differ in their judgments, then using those representations to
personalize and align LLMs. Standard practice aggregates many people's labels
into a single "gold standard," treating disagreement as noise — but on
subjective tasks, that disagreement is often meaningful, rooted in who the
annotator is and how the task is defined. I build models that preserve it
instead of averaging it away. My demographic-aware models of <span class="accent-term">annotator
disagreement</span> capture structured, group-level variation in judgments,
improving on approaches that collapse disagreement into a single answer (ACL
2026, oral). More recently, I built **VISTA**, which infers a user's values
from a few survey answers and steers a frozen LLM toward them, beating
prompt-based personalization with no added prompt tokens (under review, ARR).

<div class="pub-box" markdown="1">

## Recent Publications

- <span class="venue-tag">Under Review · ARR</span> Xu, Y., Adams, J., Hu, B., Kumar, S., Jurgens, D., & Basharat, A. (2026).
  VISTA: Steering LLMs with latent user values inferred from a few survey
  answers. [[arXiv]](https://arxiv.org/abs/2610.23702)
- <span class="venue-tag">ACL 2026 · Oral</span> Xu, Y., Derricks, V., Earl, A., & Jurgens, D. (2026). Modeling annotator
  disagreement with demographic-aware experts and synthetic perspectives.
  [[paper]](https://aclanthology.org/2026.acl-long.1914/)
- <span class="venue-tag">EMNLP 2026 · Oral</span> Xu, Y., & Jurgens, D. (2026). Beyond consensus: Perspectivist modeling and
  evaluation of annotator disagreement in NLP.
  [[arXiv]](https://arxiv.org/abs/2601.09065)
- <span class="venue-tag">NAACL 2025</span> Xu, Y., Chen, H., Rakshit, S., et al., & Jurgens, D. (2025). Causally
  modeling the linguistic and social factors that predict email response.
  [[paper]](https://aclanthology.org/2025.naacl-long.594/)

[See all publications →](/publications/)

</div>

## Currently

I'm building **B-HAP**, a hierarchical Bayesian framework that generates
per-annotator LoRA adapters from task, data, and annotator features, pooling
behavior across population, subgroup, and individual levels — extending the
same pluralistic-alignment approach behind VISTA to richer, adapter-based
personalization.


