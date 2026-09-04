---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<div class="cv-header">
  <p>
    PhD Candidate, University of Michigan &middot; NLP &amp; LLM Researcher<br>
    <a href="mailto:{{ site.author.email }}">{{ site.author.email }}</a> &middot;
    Ann Arbor, MI &middot;
    <a href="https://www.linkedin.com/in/{{ site.author.linkedin }}">LinkedIn</a> &middot;
    <a href="https://github.com/{{ site.author.github }}">GitHub</a> &middot;
    <a href="{{ site.author.googlescholar }}">Google Scholar</a>
  </p>
  <a class="btn cv-download" href="./Xu__Yinuo___Resume_public.pdf">Download PDF</a>
</div>

<section class="cv-section">
  <h2 class="cv-section-title">Education</h2>

  <div class="cv-entry">
    <div class="cv-entry-header">
      <span>University of Michigan, Ann Arbor</span>
      <span class="cv-entry-date">2023 &ndash; Present</span>
    </div>
    <div class="cv-entry-sub">Ph.D. in Information &middot; Advisor: David Jurgens</div>
  </div>

  <div class="cv-entry">
    <div class="cv-entry-header">
      <span>University of California, Berkeley</span>
      <span class="cv-entry-date">2023</span>
    </div>
    <div class="cv-entry-sub">B.A. in Data Science &amp; Statistics</div>
  </div>
</section>

<section class="cv-section">
  <h2 class="cv-section-title">Awards, Grants &amp; Leadership</h2>
  <ul class="cv-list">
    <li>Co-Organizer, <em>Personalization Without Prejudice</em> (PwP) workshop proposal under review, ACL 2026</li>
    <li>Organizer, Michigan NLP Reading Group, 2025&ndash;2026</li>
    <li>Organizer, NLP@Michigan Day 2026, 2025&ndash;2026</li>
    <li>Science Communication Fellow (selected as 1 of 20 fellows university-wide), 2023&ndash;2024</li>
    <li>University of Michigan School of Information Merit Fellowship, 2023</li>
  </ul>
</section>

<section class="cv-section">
  <h2 class="cv-section-title">Publications</h2>
  <ul class="cv-list">
    <li>Xu, Y., &amp; Jurgens, D. (2026). Beyond consensus: Perspectivist modeling and evaluation of annotator disagreement in NLP. <a href="https://arxiv.org/abs/2601.09065">EMNLP 2026</a>.</li>
    <li>Xu, Y., Derricks, V., Earl, A., &amp; Jurgens, D. (2026). Modeling annotator disagreement with demographic-aware experts and synthetic perspectives. <a href="https://aclanthology.org/2026.acl-long.1914/">ACL 2026 (oral)</a>.</li>
    <li>Xu, Y., Chen, H., Rakshit, S., et al., &amp; Jurgens, D. (2025). Causally modeling the linguistic and social factors that predict email response. <a href="https://aclanthology.org/2025.naacl-long.594/">NAACL 2025</a>. (Equal contribution)</li>
    <li>Borchers, C., Xu, Y., &amp; Pardos, Z. A. (2025). Workload overload? Late enrollment leads to course dropout. <em>Journal of Educational Data Mining</em>, 17(1), 126&ndash;156.</li>
    <li>Borchers, C., Xu, Y., &amp; Pardos, Z. A. (2024). Are you an early dropper or late shopper? Mining enrollment transaction data to study procrastination in higher education. <a href="https://educationaldatamining.org/edm2024/proceedings/2024.EDM-short-papers.41/2024.EDM-short-papers.41.pdf">EDM 2024</a>.</li>
    <li>Xu, Y., &amp; Pardos, Z. A. (2024). Extracting course similarity signal using subword embeddings. <a href="https://doi.org/10.1145/3636555.3636903">LAK 2024</a>.</li>
    <li>Xu, Y., &amp; Pardos, Z. A. (2023). Mining detailed course transaction records for semantic information. <a href="https://educationaldatamining.org/EDM2023/proceedings/2023.EDM-short-papers.39/2023.EDM-short-papers.39.pdf">EDM 2023</a>.</li>
  </ul>
  <p><a href="{{ base_path }}/publications/">&rarr; Full publication list with citations</a></p>
</section>

<section class="cv-section">
  <h2 class="cv-section-title">Relevant Experience</h2>

  <div class="cv-entry">
    <div class="cv-entry-header">
      <span>Research &amp; Development Intern, Kitware</span>
      <span class="cv-entry-date">May 2026 &ndash; Present</span>
    </div>
    <div class="cv-entry-sub">Project: Personalized LLM Steering from Inferred Value Latents</div>
    <ul>
      <li>Designed an end-to-end pipeline that infers individual users' latent value profiles from a few survey responses, with a Bayesian active-learning module adaptively selecting the most informative elicitation questions.</li>
      <li>Built a variational information-bottleneck encoder compressing responses into a low-dimensional value embedding with demographic priors for cold-start, then a hypernetwork amortizing the latent-to-steering-vector map so new users require no optimization, gated by posterior uncertainty.</li>
      <li>Evaluated against SOTA steering methods across four value datasets: +0.22 user-specific accuracy over zero-shot, outperforming existing steering methods.</li>
      <li>Ran interpretability analysis recovering a binding-vs-individualizing moral foundations axis in the learned steering vectors.</li>
    </ul>
  </div>

  <div class="cv-entry">
    <div class="cv-entry-header">
      <span>Lead Researcher, University of Michigan School of Information</span>
      <span class="cv-entry-date">Aug 2023 &ndash; Present</span>
    </div>
    <div class="cv-entry-sub">Project 1: Modeling Annotator Disagreement with Demographic-Aware Experts</div>
    <ul>
      <li>Designed Demographic-Aware Mixture-of-Experts, an interpretable architecture with demographic-aware routing to capture structured variation in annotation behavior and intersectional perspectives.</li>
      <li>Achieved state-of-the-art subgroup-level performance across five benchmark datasets, particularly under data imbalance or sparse subgroup representation.</li>
      <li>Evaluated LLM annotation reliability through zero-shot, few-shot, and LoRA-finetuned experiments, measuring alignment between persona-prompted LLM ratings and human judgments.</li>
      <li>Developed data-efficient pipelines blending real and LLM-generated synthetic annotations with alignment-weighted loss; implemented multi-GPU training workflows for model scaling and reproducibility; paper accepted at ACL 2026 (<a href="https://arxiv.org/abs/2508.02853">arXiv:2508.02853</a>).</li>
    </ul>
    <div class="cv-entry-sub">Project 2: B-HAP: Bayesian Hierarchical Adapter Personas for Situated Judgment Modeling</div>
    <ul>
      <li>Designing a hypernetwork-based framework generating parameter-efficient LoRA adapters from task, data, and annotator-feature interactions, with a three-level Bayesian hierarchy (population, subpopulation, individual) to align model behavior with group norms.</li>
      <li>Leading evaluation across a 140K-instance benchmark spanning normative, pragmatic, and preference-judgment tasks, benchmarked against Jury Learning, Mixture-of-Personas, and sociodemographic prompting baselines.</li>
    </ul>
  </div>

  <div class="cv-entry">
    <div class="cv-entry-header">
      <span>Lead Researcher, UMich School of Information &amp; Social Psychology</span>
      <span class="cv-entry-date">Aug 2023 &ndash; Present</span>
    </div>
    <div class="cv-entry-sub">Project: Measuring Racial Disparities in Doctor-Patient Conversations</div>
    <ul>
      <li>Built a large-scale annotation pipeline to evaluate doctor communication quality using a diverse pool of crowdworkers; designed and deployed a custom annotation interface to ensure demographic balance and inter-rater reliability.</li>
      <li>Developed a zero-shot LLaMA-70B annotation pipeline to label doctor behaviors (respect, formality) with prompt-engineered templates, validating alignment with human ratings.</li>
      <li>Designed and implemented a causal mediation model linking race &rarr; doctor language &rarr; respect perception &rarr; patient trust, revealing differential behavior&ndash;trust pathways across demographic groups.</li>
      <li>Paper in preparation for <em>PNAS</em>.</li>
    </ul>
  </div>

  <div class="cv-entry">
    <div class="cv-entry-header">
      <span>Graduate Research Assistant, UMich School of Information</span>
      <span class="cv-entry-date">March 2024</span>
    </div>
    <div class="cv-entry-sub">Project: Causal Modeling of Linguistic and Social Factors in Email Response (NAACL 2025)</div>
    <ul>
      <li>Co-led the development of causal inference models analyzing linguistic and social predictors of email responsiveness, combining structural equation modeling with LLM-based feature extraction.</li>
      <li>Conducted large-scale language and behavior modeling using Transformer-based encoders and mixed-effects regression to uncover latent causal drivers of social reciprocity.</li>
      <li>Presented poster at NAACL 2025; paper accepted in the main conference (<a href="https://aclanthology.org/2025.naacl-long.594/">aclanthology.org/2025.naacl-long.594</a>).</li>
    </ul>
  </div>

  <div class="cv-entry">
    <div class="cv-entry-header">
      <span>NLP Intern, Evisort (acquired by Workday)</span>
      <span class="cv-entry-date">2021</span>
    </div>
    <ul>
      <li>Developed algorithms to redact sensitive information in legal contracts using the Google DLP API and custom regex/XML pipelines.</li>
      <li>Trained and deployed LightGBM and bi-LSTM NER models in TensorFlow for contract field extraction on a SaaS platform used by enterprise clients.</li>
      <li>Designed PowerBI dashboards and PostgreSQL queries to analyze document metadata and usage patterns from AWS data sources.</li>
    </ul>
  </div>
</section>

<section class="cv-section">
  <h2 class="cv-section-title">Teaching Experience</h2>
  <ul class="cv-list">
    <li><strong>Becoming a Data Scientist</strong> (SI 568), Graduate Student Instructor, University of Michigan, Winter 2026</li>
    <li><strong>Applied Machine Learning</strong> (SI 670), Graduate Student Instructor, University of Michigan, Fall 2025</li>
    <li><strong>Natural Language Processing</strong> (Info 159/259), Teaching Assistant, UC Berkeley, Spring 2023</li>
    <li><strong>Principles and Techniques of Data Science</strong> (Data 100/200), Undergraduate Student Instructor, UC Berkeley, Fall 2022</li>
    <li><strong>Principles and Techniques of Data Science</strong> (Data 100/200), Undergraduate Student Instructor, UC Berkeley, Summer 2022</li>
    <li><strong>Technology and Social Impact</strong> (EECS 198), Lead Facilitator, UC Berkeley, Spring 2023</li>
  </ul>
</section>

<section class="cv-section">
  <h2 class="cv-section-title">Professional Service</h2>
  <ul class="cv-list">
    <li>Program Committee Member, International Conference on Computational Social Science (IC2S2), 2026</li>
    <li>Program Committee Member, Workshop on NLP and Computational Social Science (at ACL), 2026</li>
  </ul>
</section>

<section class="cv-section">
  <h2 class="cv-section-title">Technical Skills</h2>
  <p class="cv-skills">Python &middot; PyTorch &middot; Transformers &middot; vLLM &middot; Optuna &middot; ModernBERT &middot; LoRA Fine-Tuning &middot; Mixture-of-Experts &middot; Distributed / Multi-GPU Training (PyTorch DDP) &middot; Reinforcement Learning &middot; Synthetic Data Generation &middot; Causal Inference &middot; Predictive &amp; Statistical Modeling &middot; LLM Evaluation &amp; Alignment &middot; Instruction-Tuning &middot; Data Efficiency &middot; Prompt Engineering &middot; Data Pipeline Design &middot; Bayesian Modeling</p>
</section>
