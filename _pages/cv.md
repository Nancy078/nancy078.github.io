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
    PhD Candidate, University of Michigan &middot; LLM Personalization &amp; Pluralistic Alignment<br>
    <a href="mailto:{{ site.author.email }}">{{ site.author.email }}</a> &middot;
    Ann Arbor, MI &middot;
    <a href="https://www.linkedin.com/in/{{ site.author.linkedin }}">LinkedIn</a> &middot;
    <a href="https://github.com/{{ site.author.github }}">GitHub</a> &middot;
    <a href="{{ site.author.googlescholar }}">Google Scholar</a>
  </p>
  <a class="btn cv-download" href="{{ base_path }}/files/Xu__Yinuo___Resume_public.pdf">Download PDF</a>
</div>

<section class="cv-section">
  <h2 class="cv-section-title">Education</h2>

  <div class="cv-entry">
    <div class="cv-entry-header">
      <span>University of Michigan, Ann Arbor</span>
      <span class="cv-entry-date">2023 &ndash; Expected May 2028</span>
    </div>
    <div class="cv-entry-sub">Ph.D. in Information (GPA: 3.80/4.00) &middot; Advisor: David Jurgens</div>
  </div>

  <div class="cv-entry">
    <div class="cv-entry-header">
      <span>University of California, Berkeley</span>
      <span class="cv-entry-date">2023</span>
    </div>
    <div class="cv-entry-sub">B.A. in Data Science &amp; Statistics (GPA: 3.83/4.00)</div>
  </div>
</section>

<section class="cv-section">
  <h2 class="cv-section-title">Awards, Grants &amp; Leadership</h2>
  <ul class="cv-list">
    <li>Co-Organizer, <em>Personalization Without Prejudice</em> (PwP) workshop, EMNLP 2027</li>
    <li>Organizer, NLP@Michigan Day 2026, 2025&ndash;2026</li>
    <li>Organizer, Michigan NLP Reading Group, 2025&ndash;2026</li>
    <li>Science Communication Fellow (selected as 1 of 20 fellows university-wide), 2023&ndash;2024</li>
    <li>University of Michigan School of Information Merit Fellowship, 2023</li>
  </ul>
</section>

<section class="cv-section">
  <h2 class="cv-section-title">Publications (Selected)</h2>
  <ul class="cv-list">
    <li><span class="venue-tag">Under Review (ARR)</span> Xu, Y., Adams, J., Hu, B., Kumar, S., Jurgens, D., &amp; Basharat, A. (2026). VISTA: Steering LLMs with latent user values inferred from a few survey answers.</li>
    <li><a class="venue-tag" href="https://arxiv.org/abs/2601.09065">EMNLP 2026 · Oral</a> Xu, Y., &amp; Jurgens, D. (2026). Beyond consensus: Perspectivist modeling and evaluation of annotator disagreement in NLP.</li>
    <li><a class="venue-tag" href="https://aclanthology.org/2026.acl-long.1914/">ACL 2026 · Oral</a> Xu, Y., Derricks, V., Earl, A., &amp; Jurgens, D. (2026). Modeling annotator disagreement with demographic-aware experts and synthetic perspectives.</li>
    <li><a class="venue-tag" href="https://aclanthology.org/2025.naacl-long.594/">NAACL 2025</a> Xu, Y., Chen, H., Rakshit, S., et al., &amp; Jurgens, D. (2025). Causally modeling the linguistic and social factors that predict email response. (Equal contribution)</li>
  </ul>
  <p><a href="{{ base_path }}/publications/">&rarr; Full publication list with citations</a></p>
</section>

<section class="cv-section">
  <h2 class="cv-section-title">Relevant Experience</h2>

  <div class="cv-entry">
    <div class="cv-entry-header">
      <span>Research &amp; Development Intern, Kitware</span>
      <span class="cv-entry-date">May 2026 &ndash; Aug 2026</span>
    </div>
    <div class="cv-entry-sub">Project: VISTA &mdash; Steering LLMs with Latent User Values Inferred from a Few Survey Answers</div>
    <ul>
      <li>Led development of VISTA, which infers a probabilistic user-value profile from survey answers (variational encoder) and maps it via a hypernetwork to steering vectors and soft prompts to steer a frozen Llama-3-8B for personalized alignment in choice selection and free-text generation (soft prompts refined with personalized DPO). Matched or beat in-context profile prompting on 3 datasets (up to &sim;10 accuracy points) with no added prompt tokens; in free-text generation, using only survey answers, outperformed prompting with answers plus demographics, with the best net gain across minority- and majority-view users.</li>
      <li>Designed adaptive questioning that personalizes from just 6% of a survey, choosing the most informative questions and stopping automatically while keeping 94% of the full-survey accuracy gain (vs. at most 42% for standard adaptive testing).</li>
    </ul>
  </div>

  <div class="cv-entry">
    <div class="cv-entry-header">
      <span>Lead Researcher, University of Michigan School of Information</span>
      <span class="cv-entry-date">Aug 2023 &ndash; Present</span>
    </div>

    <div class="cv-entry-sub">Survey: Perspectivist Modeling of Annotator Disagreement (EMNLP 2026 &middot; Oral)</div>
    <ul>
      <li>Synthesized 110+ works on annotator disagreement in subjective, safety-relevant tasks (e.g., toxicity) into a unified taxonomy of disagreement sources and a framework of prediction targets and pooling structures, identifying the modeling gaps that motivate Project 2.</li>
    </ul>

    <div class="cv-entry-sub">Project 1: Modeling Annotator Disagreement with Demographic-Aware Experts (ACL 2026 &middot; Oral)</div>
    <ul>
      <li>Designed Demographic-Aware Mixture-of-Experts, an interpretable architecture with demographic-aware routing to capture structured variation in annotation behavior and intersectional perspectives.</li>
      <li>Achieved state-of-the-art subgroup-level performance across five benchmark datasets, improving fairness for underrepresented groups under data imbalance and sparse subgroup data.</li>
      <li>Evaluated LLM annotation reliability through zero-shot, few-shot, and LoRA-finetuned experiments, measuring alignment between persona-prompted LLM ratings and human judgments.</li>
      <li>Developed data-efficient pipelines blending real and LLM-generated synthetic annotations with alignment-weighted loss; implemented multi-GPU training workflows for model scaling and reproducibility.</li>
    </ul>

    <div class="cv-entry-sub">Project 2: Bayesian Hierarchical Adapter Personas</div>
    <ul>
      <li>Designing a hypernetwork-based framework that generates parameter-efficient LoRA adapters from task, data, and annotator-feature interactions, with a three-level Bayesian hierarchy (population, subpopulation, individual) for pluralistic alignment of model behavior with group and individual norms.</li>
      <li>Leading evaluation on a 140K-instance benchmark spanning normative, pragmatic, and preference-judgment tasks, against Jury Learning, Mixture-of-Personas, and sociodemographic prompting baselines.</li>
    </ul>

    <div class="cv-entry-sub">Project 3: Measuring Racial Disparities in Doctor-Patient Conversations</div>
    <ul>
      <li>Built a zero-shot LLaMA-70B labeling pipeline for doctor communication quality, validated against human ratings; designed a causal mediation model (doctor language &rarr; patient behavior &rarr; outcome); in prep for <em>PNAS</em>.</li>
    </ul>
  </div>

  <div class="cv-entry">
    <div class="cv-entry-header">
      <span>NLP Intern, Evisort (acquired by Workday)</span>
      <span class="cv-entry-date">May 2021 &ndash; Aug 2021</span>
    </div>
    <ul>
      <li>Trained LightGBM and bi-LSTM NER models (TensorFlow) for contract field extraction, deployed to production; built sensitive-data redaction pipelines with the Google DLP API.</li>
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
  <p class="cv-skills">Python &middot; PyTorch &middot; Hugging Face Transformers &middot; PEFT / LoRA &middot; vLLM &middot; SLURM &middot; Git &middot; Hypernetworks &middot; Activation Steering &middot; DPO &middot; Mixture-of-Experts &middot; Multi-GPU Training (DDP) &middot; Bayesian &amp; Variational Inference &middot; Causal Inference &middot; LLM Evaluation &amp; Alignment &middot; Optuna</p>
</section>
