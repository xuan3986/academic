---
title: 'UDDETTS: Unifying Discrete and Dimensional Emotions for Controllable Emotional Text-to-Speech'

authors:
  - admin
  - et al.

date: '2025-09-01T00:00:00Z'
doi: ''
publishDate: '2026-06-11T00:00:00Z'

publication_types: ['article']
publication: 'Long paper (under review at *ICLR 2026*)'
publication_short: 'ICLR 2026 (under review)'

abstract: |-
  Recent LLM-based TTS models have achieved striking gains in expressive speech synthesis, yet they still struggle to produce **fine-grained, interpretable emotional speech**. Conventional methods rely on discrete emotion labels to control category and intensity, which cannot capture the complexity and continuity of human emotional perception. Moreover, the lack of large-scale emotional speech datasets with balanced distributions and fine-grained emotional annotations often causes overfitting and impedes effective emotion control.

  To address these issues, we propose **UDDETTS**, a universal LLM framework that unifies **discrete and dimensional emotions** for controllable emotional TTS. UDDETTS introduces the interpretable **Arousal–Dominance–Valence (ADV)** space and supports control via either discrete emotion labels or non-linearly quantized **ADV tokens**, enabling fine-grained, decoupled emotion control beyond traditional label-based methods. The framework comprises a neural codec language model, an OT-CFM module with an emotional mixture encoder, and a vocoder, augmented with an **ADV predictor** that enables end-to-end synthesis even when explicit annotations are unavailable. A **semi-supervised training strategy** unifies spontaneous and elicited emotional speech datasets — fusing label-only and ADV-annotated data — to mitigate emotional imbalance and the low controllable coverage of the ADV space. Across label-controlled, ADV-controlled, and end-to-end emotional TTS, UDDETTS achieves linear emotion control along three interpretable dimensions and significantly outperforms strong LLM-based TTS baselines.

summary: |-
  A universal LLM-based TTS framework unifying discrete labels and the continuous Arousal–Dominance–Valence space, with semi-supervised training and an ADV predictor for fine-grained, interpretable emotion control.

tags:
  - Emotional TTS
  - Speech LLM
  - Controllable Generation
  - Arousal–Dominance–Valence
  - Semi-Supervised Learning

featured: true

links:
  - name: OpenReview
    url: https://openreview.net/forum?id=DuPYSaCiep
  - name: Demo & Code
    url: https://anonymous.4open.science/w/UDDETTS

url_pdf: 'https://openreview.net/pdf?id=DuPYSaCiep'
url_code: 'https://anonymous.4open.science/w/UDDETTS'
url_dataset: ''
url_poster: ''
url_project: 'https://anonymous.4open.science/w/UDDETTS'
url_slides: ''
url_source: ''
url_video: ''

image:
  caption: ''
  focal_point: ''
  preview_only: false

projects: []
slides: ''
---
