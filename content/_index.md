---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  # - block: skills
  #   content:
  #     title: Skills
  #     text: ''
  #     # Choose a user to display skills from (a folder name within `content/authors/`)
  #     username: admin
  #   design:
  #     columns: '1'
  - block: experience
    id: education
    content:
      title: Education
      date_format: Jan 2006
      # Education timeline.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current school.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: M.Eng. in Information and Communication Engineering
          company: University of Science and Technology of China (USTC)
          company_url: 'https://www.ustc.edu.cn/'
          company_logo: ustc
          location: Hefei, China
          date_start: '2024-09-03'
          date_end: ''
          description: |2-
              * School of Information Science and Technology, NERC-SLIP.
              * Research focus: text-to-speech, expressive & emotional speech synthesis, multimodal dubbing, speech foundation models.
              * 2024 First-Class Academic Scholarship; 2025 Zenghua Special Scholarship; 2025 USTC 0006 Scholarship.
              * Secretary of the 2nd Postgraduate Party Branch, Class of 2024, School of Information Science and Technology (Department 6).
        - title: B.Eng. in Computer Science and Technology
          company: Northwestern Polytechnical University (NWPU)
          company_url: 'https://www.nwpu.edu.cn/'
          company_logo: nwpu
          location: Xi'an, China
          date_start: '2020-09-01'
          date_end: '2024-06-28'
          description: |2-
              * **Comprehensive score ranked 1 / 234**, recommended for admission to USTC.
              * **Outstanding Graduate** of NWPU; 2021–2023 Outstanding Student of NWPU.
              * 2020–2024 Class Study Committee Member — led the class to the No. 1 average GPA in the major for two consecutive years.
              * 2020–2021 Member of the school-level student union; college peer mentor.
              * 2020–2021 School of Physical Science and Technology, General Physics Class.
              * 2021–2024 School of Computer Science, Computer Science and Technology.
              * Internships: ASLP@NPU Lab (2022), Huawei (2023), iFLYTEK Co., Ltd. (2023–2024).
        - title: Senior High School (Chemistry Olympiad Class)
          company: Hengshui High School
          company_url: 'https://hbhszx.cn/'
          company_logo: zh
          location: Hebei, China
          date_start: '2017-07-01'
          date_end: '2020-07-01'
          description: |2-
              * 2019 First Prize, 33rd Chinese Chemistry Olympiad.
              * 2020 663 points in the National College Entrance Examination (Gaokao).
    design:
      columns: '2'

  - block: experience
    id: experience
    content:
      title: Research & Internship Experience
      date_format: Jan 2006
      items:
        - title: Speech Foundation Model Pre-training Intern
          company: Xiaomi · MiMo Team
          company_url: ''
          company_logo: ''
          location: ''
          date_start: '2026-05-01'
          date_end: ''
          description: |2-
              * Pre-training of speech foundation models on hundreds of millions of hours of data.
              * Multimodal understanding and unified audio synthesis.
        - title: Algorithm Engineer Intern (Speech AI)
          company: Alibaba Cloud · Tongyi Lab
          company_url: ''
          company_logo: ''
          location: ''
          date_start: '2025-07-01'
          date_end: '2026-05-01'
          description: |2-
              * Participated in emotional TTS training of **CosyVoice3-0.5B**.
              * Led an algorithm research project on a multimodal large model for **movie dubbing**, proposing **Fun-CineForge** — an end-to-end pipeline for large-scale multimodal dubbing data plus a dubbing model designed for diverse cinematic scenes.
              * Built and open-sourced **CineDub**, the first movie-dubbing dataset, from scratch.
              * Across monologue, narration, dialogue, and complex multi-speaker scenes, Fun-CineForge surpasses SOTA in audio quality, temporal alignment, lip-sync, timbre similarity, and instruction following. It is the first model that relies on the **temporal modality** for time alignment and supports long-video dubbing in diverse scenarios.
              * First-author **Oral paper at IJCAI–ECAI 2026** — *FunCineForge: A Unified Dataset Pipeline and Model for Zero-Shot Movie Dubbing in Diverse Cinematic Scenes*. Open-sourced in Alibaba Tongyi's official speech repository (10K+ downloads); demos on HuggingFace and ModelScope. Project site: <https://funcineforge.github.io/>.
        - title: NSFC Joint Fund Project — Interpretable Emotional Prosody Modeling and Control for TTS
          company: USTC · NERC-SLIP
          company_url: 'http://nelslip.ustc.edu.cn/'
          company_logo: ustc
          location: Hefei, China
          date_start: '2024-11-01'
          date_end: '2025-06-30'
          description: |2-
              * Conventional emotional TTS relies on discrete emotion labels, which fail to capture the complexity and continuity of human emotional perception, and large-scale corpora with balanced and fine-grained emotion annotation are scarce.
              * Proposed **UDDETTS**, a unified framework that fuses discrete and dimensional emotion, introducing the interpretable **Arousal–Dominance–Valence (ADV)** space for dimensional emotion description.
              * Supports emotion control driven by either discrete labels or non-linearly quantized ADV values; disentangles speech emotion along three psychological dimensions and achieves **fine-grained linear 3-D controllability**.
              * Significantly outperforms baselines in naturalness and emotion control accuracy; demonstrates the superiority of the ADV space for end-to-end emotional TTS.
              * First-author paper: *UDDETTS: Unifying Discrete and Dimensional Emotions for Controllable Emotional Text-to-Speech*.
        - title: Acoustic Modeling for Diverse and Controllable Prosodic TTS (Joint with iFLYTEK & China Mobile Research)
          company: USTC · NERC-SLIP / iFLYTEK / China Mobile Research
          company_url: ''
          company_logo: ustc
          location: Hefei, China
          date_start: '2024-06-01'
          date_end: '2024-10-30'
          description: |2-
              * Proposed **DiffStyleTTS**, a hierarchical prosody modeling framework for TTS based on a **conditional diffusion model** and an improved classifier-free guidance strategy.
              * Achieved superior results in **naturalness, prosody transfer, and prosody control**, with both diversity and controllability.
              * First-author **long paper with Oral** presentation at **COLING 2025** — *DiffStyleTTS: Diffusion-based Hierarchical Prosody Modeling for Text-to-Speech with Diverse and Controllable Styles*.
        - title: Assistant Algorithm Researcher Intern (Speech Synthesis) — Undergraduate Thesis
          company: iFLYTEK Co., Ltd. · Core R&D Platform
          company_url: 'https://www.iflytek.com/'
          company_logo: ''
          location: Hefei, China
          date_start: '2023-12-01'
          date_end: '2024-04-30'
          description: |2-
              * Researched diffusion-model-based acoustic models for diverse and controllable prosodic TTS.
              * Completed undergraduate graduation thesis on this work.
        - title: Research Intern — Expressive Audiobook Speech Synthesis
          company: Huawei
          company_url: ''
          company_logo: ''
          location: ''
          date_start: '2023-06-01'
          date_end: '2023-07-31'
          description: |2-
              * Worked on *Modeling High-Expressive Continuous Emotional Space for Audiobooks*, addressing listener fatigue caused by the limitations of explicit, discrete emotion categories.
              * Built a **multimodal emotional space** and proposed a cross-modal supervised text-emotion perception module based on **T5** and **contrastive learning** — significantly improving emotional similarity.
              * Work titled *Text-aware and Context-aware Expressive Audiobook Speech Synthesis*.
        - title: Research Intern (Singing Voice Synthesis)
          company: Shaanxi Provincial Key Lab of Speech & Image Information Processing — ASLP@NPU
          company_url: ''
          company_logo: ''
          location: Xi'an, China
          date_start: '2022-06-01'
          date_end: '2022-07-31'
          description: |2-
              * Contributed to the **Opencpop** dataset construction and **ByteSing**-based singing voice synthesis model training.
              * Optimized the Duration / LF0 / U-V Predictor with **BLSTM** to capture long-term temporal dependency, significantly reducing F0 error and improving audio quality.
              * Awarded **Outstanding Intern of the ASLP Lab**.
    design:
      columns: '2'

  - block: accomplishments
    id: awards
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Scholarships'
      subtitle:
      # Date format: https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: ''
          date_end: ''
          date_start: '2025-12-30'
          description: ''
          icon: ustc
          organization: University of Science and Technology of China
          organization_url: 'https://www.ustc.edu.cn/'
          title: USTC 0006 Scholarship
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2025-12-30'
          description: ''
          icon: ustc
          organization: University of Science and Technology of China
          organization_url: 'https://www.ustc.edu.cn/'
          title: Zenghua Special Scholarship
          url: ''
        - certificate_url: 'uploads/2024硕士一等学业奖学金.jpg'
          date_end: ''
          date_start: '2024-10-30'
          description: ''
          icon: ustc
          organization: University of Science and Technology of China
          organization_url: 'https://www.ustc.edu.cn/'
          title: Master's First-Class Academic Scholarship (2024–2025)
          url: ''
        - certificate_url: 'uploads/小米优秀专项奖学金.jpg'
          date_end: ''
          date_start: '2023-12-30'
          description: ''
          icon: nwpu
          organization: Northwestern Polytechnical University & Xiaomi Corporation
          organization_url: ''
          title: Xiaomi Excellent Scholarship
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2023-12-30'
          description: ''
          icon: nwpu
          organization: Ministry of Education of the People's Republic of China
          organization_url: ''
          title: National Inspirational Scholarship (2022, 2023)
          url: ''
        - certificate_url: 'uploads/吴亚军专项奖学金.jpg'
          date_end: ''
          date_start: '2022-12-30'
          description: ''
          icon: nwpu
          organization: Northwestern Polytechnical University
          organization_url: 'https://www.nwpu.edu.cn/'
          title: Yajun Wu Special Scholarship
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2023-12-30'
          description: ''
          icon: nwpu
          organization: Northwestern Polytechnical University
          organization_url: 'https://www.nwpu.edu.cn/'
          title: NWPU First-Class Academic Scholarship (2021–2023)
          url: ''
        - certificate_url: 'uploads/国家奖学金.jpg'
          date_end: ''
          date_start: '2021-12-30'
          description: ''
          icon: ''
          organization: Ministry of Education of the People's Republic of China
          organization_url: ''
          title: National Scholarship
          url: ''
    design:
      columns: '2'
  - block: accomplishments
    content:
      title: 'Competitions (Selected)'
      subtitle:
      date_format: Jan 2006
      items:
        - certificate_url: 'uploads/MCM.png'
          date_end: ''
          date_start: '2023-12-30'
          description: 'Outstanding Winner / Finalist Award'
          icon: COMAP
          organization: The Consortium for Mathematics and Its Applications (COMAP)
          organization_url: 'https://www.comap.com/'
          title: Mathematical Contest in Modeling (MCM) — Outstanding Winner
          url: 'https://www.comap.com/contests/mcm-icm'
        - certificate_url: 'uploads/CUMCM.jpg'
          date_end: ''
          date_start: '2022-12-30'
          description: ''
          icon: cumcm
          organization: China Society for Industrial and Applied Mathematics (CSIAM)
          organization_url: 'https://www.csiam.org.cn/'
          title: Contemporary Undergraduate Mathematical Contest in Modeling (CUMCM) — Shaanxi First Prize
          url: 'https://www.mcm.edu.cn/'
        - certificate_url: 'uploads/CUPT-Ind.jpg'
          date_end: ''
          date_start: '2021-07-05'
          description: ''
          icon: CUPT
          organization: The Chinese Physical Society (CPS)
          organization_url: 'http://www.cps-net.org.cn/'
          title: China Undergraduate Physics Tournament (CUPT) — Shaanxi Individual First Prize
          url: 'https://www.cupt-iypt.com/'
        - certificate_url: 'uploads/CUPT-Team.jpg'
          date_end: ''
          date_start: '2021-07-05'
          description: ''
          icon: CUPT
          organization: The Chinese Physical Society (CPS)
          organization_url: 'http://www.cps-net.org.cn/'
          title: China Undergraduate Physics Tournament (CUPT) — Shaanxi Team First Prize
          url: 'https://www.cupt-iypt.com/'
        - certificate_url: 'uploads/wenxin.jpg'
          date_end: ''
          date_start: '2022-10-10'
          description: ''
          icon: wenxin
          organization: Baidu Wenxin
          organization_url: 'https://wenxin.baidu.com/'
          title: Baidu Wenxin LLM Creative Application — A- Award
          url: 'https://wenxin.baidu.com/younger'
        - certificate_url: ''
          date_end: ''
          date_start: '2022-09-05'
          description: ''
          icon: nwpu
          organization: Communist Youth League of China · Shaanxi
          organization_url: ''
          title: '"Challenge Cup" Shaanxi Undergraduate Entrepreneurship Plan Competition — Bronze Award'
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2022-09-05'
          description: ''
          icon: nwpu
          organization: Northwestern Polytechnical University
          organization_url: 'https://en.nwpu.edu.cn/'
          title: NWPU Programming Competition — First Prize
          url: 'https://jiaowu.nwpu.edu.cn/info/1160/8306.htm'
        - certificate_url: 'uploads/math.jpg'
          date_end: ''
          date_start: '2021-11-30'
          description: ''
          icon: nwpu
          organization: Northwestern Polytechnical University
          organization_url: 'https://en.nwpu.edu.cn/'
          title: NWPU Undergraduate Mathematics Competition — First Prize
          url: ''
        - certificate_url: 'uploads/physics.jpg'
          date_end: ''
          date_start: '2021-05-30'
          description: ''
          icon: nwpu
          organization: Northwestern Polytechnical University
          organization_url: 'https://en.nwpu.edu.cn/'
          title: NWPU Physics Experiment Competition — First Prize
          url: 'https://physics.nwpu.edu.cn/info/1051/2013.htm'
    design:
      columns: '2'
  - block: accomplishments
    content:
      title: 'Other Honors (Selected)'
      subtitle:
      date_format: Jan 2006
      items:
        - certificate_url: ''
          date_end: ''
          date_start: '2026-06-30'
          description: ''
          icon: ustc
          organization: University of Science and Technology of China
          organization_url: 'https://www.ustc.edu.cn/'
          title: Outstanding Communist Party Member (2026)
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2025-06-30'
          description: ''
          icon: ustc
          organization: University of Science and Technology of China
          organization_url: 'https://www.ustc.edu.cn/'
          title: Outstanding Communist Party Member (2025)
          url: ''
        - certificate_url: 'uploads/CN116630684B.PDF'
          date_end: ''
          date_start: '2025-04-01'
          description: 'A Lightweight End-to-End Object Segmentation Method for Road Damage Detection.'
          icon: zhuanli
          organization: China National Intellectual Property Administration
          organization_url: 'https://www.cnipa.gov.cn/'
          title: Granted Chinese Invention Patent
          url: 'https://pss-system.cponline.cnipa.gov.cn/conventionalSearch'
        - certificate_url: 'uploads/优秀毕业生.pdf'
          date_end: ''
          date_start: '2024-06-30'
          description: ''
          icon: nwpu
          organization: Northwestern Polytechnical University
          organization_url: 'https://en.nwpu.edu.cn/'
          title: Outstanding Graduate of NWPU
          url: 'https://mp.weixin.qq.com/s/9-KtgJ1bb4zE3UM3gUthdA'
        - certificate_url: 'uploads/2023优秀大学生.jpg'
          date_end: ''
          date_start: '2023-12-30'
          description: ''
          icon: nwpu
          organization: Northwestern Polytechnical University
          organization_url: 'https://en.nwpu.edu.cn/'
          title: Outstanding Student of NWPU (2021, 2022, 2023)
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2022-05-04'
          description: ''
          icon: nwpu
          organization: Communist Youth League of China · NWPU
          organization_url: ''
          title: 'May 4th Honors — Outstanding Communist Youth League Member (2021, 2022)'
          url: ''
        - certificate_url: 'uploads/ASLP.jpg'
          date_end: ''
          date_start: '2022-09-01'
          description: ''
          icon: aslp
          organization: ASLP@NPU Lab — Shaanxi Provincial Key Lab of Speech & Image Information Processing
          organization_url: ''
          title: Outstanding Intern, "AI Intelligent Speech Internship Program"
          url: ''
        - certificate_url: 'uploads/十四运.jpg'
          date_end: ''
          date_start: '2021-10-30'
          description: ''
          icon: shisiyun
          organization: General Administration of Sport / Communist Youth League Central Committee
          organization_url: 'https://www.sport.gov.cn/n4/n23367606/index.html'
          title: 14th National Games of the PRC — Flag Phalanx (Commendation by the State Council & CYLC Central Committee)
          url: 'https://news.nwpu.edu.cn/info/1002/78675.htm'
    design:
      columns: '2'
  - block: collection
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: compact
      columns: '2'
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: Computer Vision
          tag: Computer Vision
        - name: Scientific Computing
          tag: Scientific Computing
        - name: LLM
          tag: LLM
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  - block: markdown
    id: service
    content:
      title: Service & Activities
      subtitle: ''
      text: |-
        - **2024 – Present:** Secretary of the 2nd Postgraduate Party Branch, Class of 2024, School of Information Science and Technology (Department 6), USTC.
        - **2020 – 2024:** Class Study Committee Member at NWPU — led the class to the No. 1 average GPA in the major for two consecutive years.
        - **2021.08 – 2021.10:** Served on the flag phalanx for the opening and closing ceremonies of the **14th National Games of the PRC**; commended by the State Council and the Central Committee of the Communist Youth League of China.
        - **2020 – 2024:** Participated in 10+ social-practice / volunteer programs, with **917 hours** of total volunteer service.
    design:
      columns: '2'
  - block: tag_cloud
    content:
      title: Popular Topics
    design:
      columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        If you are interested in my research or would like to collaborate, please feel free to reach out.
      # Contact (add or remove contact options as necessary)
      email: jxliu@mail.ustc.edu.cn
      phone: 18803383986
      # appointment_url:
      address:
        street: No.100, Fuxing Road
        city: HeFei
        region: Shushan District
        postcode: '230031'
        country: China
        country_code: CH
      directions: Enter Xin Zhi Building
      office_hours: 'Working days 10:00-17:00'
      # Choose a map provider in `params.yaml` to show a map from these coordinates
      coordinates:
        latitude: '31.82447164209566'
        longitude: '117.12452094557694'
      contact_links:
        - icon: github
          icon_pack: fab
          name: GitHub
          link: 'https://github.com/xuan3986'
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/xuan3986'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
---
