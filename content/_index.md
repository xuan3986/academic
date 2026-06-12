---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  # ─────────────────────────  Biography  ─────────────────────────
  - block: about.biography
    id: about
    content:
      title: Biography
      username: admin

  # ─────────────────────────  Education  ─────────────────────────
  - block: experience
    id: education
    content:
      title: Education
      date_format: Jan 2006
      items:
        - title: M.Eng. in Information & Communication Engineering
          company: University of Science and Technology of China · NERC-SLIP
          company_url: 'http://nelslip.ustc.edu.cn/'
          company_logo: ustc
          location: Hefei, China
          date_start: '2024-09-03'
          date_end: ''
          description: Research on text-to-speech, expressive & emotional synthesis, multimodal dubbing, and speech foundation models.
        - title: B.Eng. in Computer Science & Technology
          company: Northwestern Polytechnical University
          company_url: 'https://www.nwpu.edu.cn/'
          company_logo: nwpu
          location: Xi'an, China
          date_start: '2020-09-01'
          date_end: '2024-06-28'
          description: Comprehensive score ranked **1 / 234** · Outstanding Graduate · recommended for admission to USTC.
        - title: Senior High School (Chemistry Olympiad Class)
          company: Hengshui High School
          company_url: 'https://hbhszx.cn/'
          company_logo: zh
          location: Hebei, China
          date_start: '2017-07-01'
          date_end: '2020-07-01'
          description: First Prize, 33rd Chinese Chemistry Olympiad.
    design:
      columns: '2'

  # ───────────────────  Research & Internship  ───────────────────
  - block: experience
    id: experience
    content:
      title: Research & Internship Experience
      date_format: Jan 2006
      items:
        - title: Speech Foundation Model Pre-training Intern
          company: Xiaomi · MiMo Team
          company_logo: xiaomi
          location: ''
          date_start: '2026-05-01'
          date_end: ''
          description: Pre-training a speech foundation model on hundreds of millions of hours of data — multimodal understanding & unified audio synthesis.
        - title: Algorithm Engineer Intern — Fun-CineForge
          company: Alibaba Cloud · Tongyi Lab
          company_logo: aliyun
          location: ''
          date_start: '2025-07-01'
          date_end: '2026-05-01'
          description: Led **Fun-CineForge** — a unified pipeline + multimodal model for zero-shot movie dubbing, plus the open-source **CineDub** dataset. Contributed to emotional-TTS training of CosyVoice3-0.5B. *(IJCAI–ECAI 2026 Oral, 10K+ downloads.)*
        - title: NSFC Joint-Fund Project · UDDETTS
          company: USTC · NERC-SLIP
          company_url: 'http://nelslip.ustc.edu.cn/'
          company_logo: ustc
          location: Hefei, China
          date_start: '2024-11-01'
          date_end: '2025-06-30'
          description: A unified discrete + dimensional (Arousal–Dominance–Valence) emotional-TTS framework with fine-grained linear 3-D controllability.
        - title: NSFC Joint-Fund Project · DiffStyleTTS
          company: USTC · NERC-SLIP
          company_url: 'http://nelslip.ustc.edu.cn/'
          company_logo: ustc
          location: Hefei, China
          date_start: '2024-06-01'
          date_end: '2024-10-30'
          description: Diffusion-based hierarchical prosody modeling for diverse and controllable TTS. *(COLING 2025 Oral.)*
        - title: Research Intern · Undergraduate Thesis
          company: iFLYTEK · Core R&D Platform
          company_url: 'https://www.iflytek.com/'
          company_logo: iflytek
          location: Hefei, China
          date_start: '2023-12-01'
          date_end: '2024-04-30'
          description: Diffusion-based acoustic models for diverse and controllable prosodic TTS.
        - title: Research Intern · Expressive Audiobook TTS
          company: Huawei
          company_logo: huawei
          location: ''
          date_start: '2023-06-01'
          date_end: '2023-07-31'
          description: A multi-modal continuous emotional space + T5/contrastive text-emotion module to relieve audiobook listener fatigue.
        - title: Research Intern · Singing Voice Synthesis
          company: ASLP@NPU Lab
          company_logo: nwpu
          location: Xi'an, China
          date_start: '2022-06-01'
          date_end: '2022-07-31'
          description: Contributed to the **Opencpop** dataset; optimised ByteSing's Duration / LF0 / U-V Predictor with BLSTM. Outstanding Intern of ASLP Lab.
    design:
      columns: '2'

  # ─────────────────  Projects  ─────────────────
  - block: collection
    id: featured
    content:
      title: Projects
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card

  # ─────────────────────  Honors & Awards  ─────────────────────
  - block: markdown
    id: awards
    content:
      title: Honors & Awards
      subtitle: ''
      text: |-
        ### 🎓 Scholarships
        - **Zenghua Special Scholarship**, USTC · 2025
        - **USTC 0006 Scholarship** · 2025
        - **Master's First-Class Academic Scholarship**, USTC · 2024, 2025
        - **Xiaomi Excellent Scholarship** · 2023
        - **National Inspirational Scholarship** · 2022, 2023
        - **Yajun Wu Special Scholarship**, NWPU · 2022
        - **First-Class Academic Scholarship**, NWPU · 2021, 2022, 2023
        - **National Scholarship** · 2021

        ### 🏆 Competitions (Selected)
        - **Mathematical Contest in Modeling (MCM)** — Outstanding Winner · 2023
        - **CUMCM** — Shaanxi First Prize · 2022
        - **CUPT** — Shaanxi Individual & Team First Prize · 2021
        - **Baidu Wenxin LLM Creative Application** — A- Award · 2022
        - **"Challenge Cup"** Shaanxi Entrepreneurship Plan — Bronze · 2022
        - **NWPU Programming / Mathematics / Physics Experiment** — First Prize

        ### ✨ Other Honors
        - **Outstanding Communist Party Member**, USTC · 2025, 2026
        - **Granted Chinese Invention Patent** — Lightweight End-to-End Object Segmentation for Road-Damage Detection · 2025
        - **[Outstanding Graduate of NWPU](https://mp.weixin.qq.com/s/9-KtgJ1bb4zE3UM3gUthdA)** · 2024
        - **Outstanding Student of NWPU** · 2021, 2022, 2023
        - **Outstanding Communist Youth League Member** (May 4th Honors) · 2021, 2022
        - **Outstanding Intern**, ASLP@NPU Lab · 2022
        - **14th National Games of the PRC — Flag Phalanx**, commended by the State Council & CYLC Central Committee · 2021
    design:
      columns: '2'

  # ────────────────────  Service & Activities  ────────────────────
  - block: markdown
    id: service
    content:
      title: Service & Activities
      subtitle: ''
      text: |-
        - Secretary, **2nd Postgraduate Party Branch**, Class of 2024, School of Information Science and Technology, USTC · 2024 – Present
        - **Class Study Committee Member**, NWPU · 2020 – 2024
    design:
      columns: '2'

  # ─────────────────────────  Contact  ─────────────────────────
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle: ''
      text: |-
        Open to collaboration in speech synthesis, multimodal generation, and speech foundation models — feel free to reach out.
      email: jxliu@mail.ustc.edu.cn
      phone: 18803383986
      address:
        street: No.100, Fuxing Road
        city: Hefei
        region: Shushan District
        postcode: '230031'
        country: China
        country_code: CN
      directions: ''
      coordinates:
        latitude: '31.82447164209566'
        longitude: '117.12452094557694'
      contact_links:
        - icon: github
          icon_pack: fab
          name: GitHub
          link: 'https://github.com/xuan3986'
      autolink: true
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          captcha: false
    design:
      columns: '2'
---
