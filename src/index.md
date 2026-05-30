---
layout: layouts/base.njk
title: Home
---

<section class="vast-hero" id="top" aria-labelledby="vast-title">
  <div class="wrapper">
    <div class="vast-hero-content">
      <h1 id="vast-title">{% for line in site.workshopNameLines %}<span>{{ line }}</span>{% endfor %}</h1>
      <p class="vast-lead">{{ site.description }}</p>
      <div class="vast-meta" aria-label="Workshop details">
        <span>{{ site.coLocated | safe }}</span>
        <span>📍 {{ site.location }}</span>
        <span>📅 {{ site.date }}</span>
      </div>
    </div>
  </div>
</section>

<div class="wrapper content-wrapper">

#### About

Large language model agents are rapidly becoming active participants in software engineering (SE), assisting with code generation, testing, debugging, program repair, maintenance, DevOps, documentation, and security analysis. However, current designs and evaluations often focus on final outputs while leaving agents' intermediate reasoning, context use, tool interactions, and failure modes insufficiently examined.

This creates a critical trust gap: software engineers need to understand not only whether an agent completes a task, but whether its behavior is verifiable, aligned with developer intent, and secure under open-world adversarial conditions.

VAST 2027 aims to establish a research agenda for trustworthy SE agents. The workshop will bring together researchers and practitioners from software engineering, program analysis, testing, formal methods, security, human-AI collaboration, and trustworthy AI. Topics include agent traces, evidence-grounded reasoning, trace-based verification, red-teaming, prompt/context injection, guardrails, runtime monitoring, human review, alignment with project policies, and benchmarks for trustworthy agentic SE workflows.

<figure class="architecture-figure">
  <img src="{{ site.baseUrl }}/assets/img/architecture.jpg" alt="Overview of trustworthy agentic software engineering, including SE agent tasks, reasoning traces, context use, tool calls, evidence, human review, runtime monitoring, verifiability, alignment, and security.">
</figure>

---

#### Important Dates

All dates are 23:59:59 AoE (UTC-12h), unless otherwise stated.

<ul class="dates-list">
{% for item in dates %}
  <li>
    <span class="date-icon" aria-hidden="true">{{ item.icon }}</span>
    <span class="date-event">{{ item.event }}</span>
    <span class="date-value">{{ item.date }}</span>
  </li>
{% endfor %}
</ul>

</div>
