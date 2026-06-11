---
title: 'Fun-CineForge: A Unified Dataset Pipeline and MLLM-based Model for Zero-Shot Movie Dubbing in Diverse Cinematic Scenes'

authors:
  - admin
  - et al.

date: '2026-08-01T00:00:00Z'
doi: ''
publishDate: '2026-06-11T00:00:00Z'

publication_types: ['paper-conference']
publication: In *Proceedings of IJCAI–ECAI 2026* — **Oral**
publication_short: In *IJCAI–ECAI 2026 (Oral)*

abstract: |-
  Movie dubbing synthesizes speech from scripts conditioned on video scenes, requiring accurate lip sync, faithful timbre transfer, and proper modeling of character identity and emotion. Existing approaches face two major limitations: (1) high-quality multimodal dubbing datasets are limited in scale, suffer from high word-error rates, sparse annotations, costly manual labeling, and are restricted to monologue scenes; (2) existing dubbing models rely solely on the lip region for audio–visual alignment, limiting them in complex live-action scenes and yielding suboptimal lip sync, speech quality, and emotional expressiveness.

  We propose **Fun-CineForge**, comprising an **end-to-end production pipeline** for large-scale dubbing datasets and an **MLLM-based dubbing model** designed for diverse cinematic scenes. Using the pipeline we construct **CineDub**, the first Chinese television dubbing dataset with rich annotations. Across monologue, narration, dialogue, and complex multi-speaker scenes, Fun-CineForge consistently outperforms SOTA methods in audio quality, lip sync, timbre transfer, and instruction following — and is the first dubbing model to align long videos via the temporal modality. The model has been open-sourced through Alibaba Tongyi's official speech repository (10K+ downloads), with releases on GitHub, Hugging Face, and ModelScope.

summary: |-
  A unified end-to-end pipeline (CineDub dataset) and MLLM-based model for zero-shot movie dubbing across diverse cinematic scenes — open-sourced via Alibaba Tongyi.

tags:
  - Speech Synthesis
  - Movie Dubbing
  - Multimodal LLM
  - Zero-Shot

featured: true

links:
  - name: Project Site
    url: https://funcineforge.github.io/
  - name: GitHub
    url: https://github.com/FunAudioLLM/FunCineForge
  - name: Hugging Face
    url: https://huggingface.co/FunAudioLLM/Fun-CineForge
  - name: ModelScope
    url: https://www.modelscope.cn/models/FunAudioLLM/Fun-CineForge

url_pdf: ''
url_code: 'https://github.com/FunAudioLLM/FunCineForge'
url_dataset: 'https://funcineforge.github.io/#dataset'
url_poster: ''
url_project: 'https://funcineforge.github.io/'
url_slides: ''
url_source: ''
url_video: 'https://funcineforge.github.io/#demo'

image:
  caption: ''
  focal_point: ''
  preview_only: false

projects: []
slides: ''
---
