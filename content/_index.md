---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: hero
    demo: true # Only display this section in the Hugo Blox Builder demo site
    content:
      title: Hugo Academic Theme
      image:
        filename: hero-academic.png
      cta:
        label: '**Get Started**'
        url: https://hugoblox.com/templates/
      cta_alt:
        label: Ask a question
        url: https://discord.gg/z8wNYzb
      cta_note:
        label: >-
          <div style="text-shadow: none;"><a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star">Star Hugo Blox Builder</a></div><div style="text-shadow: none;"><a class="github-button" href="https://github.com/HugoBlox/theme-academic-cv" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star">Star the Academic template</a></div>
      text: |-
        **Generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 500,000+ sites.**

        **Easily build anything with blocks - no-code required!**

        From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.

        <!--Custom spacing-->
        <div class="mb-3"></div>
        <!--GitHub Button JS-->
        <script async defer src="https://buttons.github.io/buttons.js"></script>
    design:
      background:
        gradient_end: '#1976d2'
        gradient_start: '#004ba0'
        text_color_light: true
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
    id: experience
    content:
      title: Experience
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Senior School
          company: Hengshui High School
          company_url: 'https://hbhszx.cn/'
          company_logo: zh
          location: Hebei, China
          date_start: '2017-07-01'
          date_end: '2020-07-01'
          description: |2-
              * 2019 Frist prize in the 33rd Chinese Chemistry Olympiad.
              * 2020 663 points in the national college entrance examination.
        - title: Undergraduate
          company: Northwestern Polytechnical University
          company_url: 'https://www.nwpu.edu.cn/'
          company_logo: nwpu
          location: Xi'an, China
          date_start: '2020-09-01'
          date_end: '2024-06-28'
          description: |2-
              * 2020-2024 Study committee.
              * 2020-2021 School-level student union member, college peer mentor.
              * 2020-2021 School of Physical Science and Technology, Physics general class.
              * 2021-2024 School of Computer Science, Computer Science and Technology.
              * 2021 National Scholarship.
              * 2022-2023 National Inspirational Scholarship.
              * 2022 Yajun Wu Special Scholarship.
              * 2023 Xiaomi Excellent Scholarship.
              * 2021-2023 First Class Academic Scholarship.
              * 2022 Jun.-Aug. Excellent intern at ASLP@NPU lab.
              * 2023 Jun.-Aug. Intern at Huawei.
              * 2023 Nov.-2024 Apr. Intern at iFLYTEK Co.Ltd.
              * Outstanding Graduate of Northwestern Polytechnical University.
              * Ranked first in comprehensive score, recommended for admission to the University of Science and Technology of China.
        - title: Postgraduate
          company: University of Science and Technology of China
          company_url: 'https://www.ustc.edu.cn/'
          company_logo: ustc
          location: Hefei, China
          date_start: '2024-09-03'
          date_end: '2027-06-30'
          description: |2-
              * 2024-now Party branch secretary.
              * 2024-now School of information science and technology, Information and Communication Engineering.
              * 2024-now Engaged in TTS research in NERCSLIP.
              * 2024 First Class Academic Scholarship.
    design:
      columns: '2'

  - block: accomplishments
    id: awards
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Scholarship (Partial)'
      subtitle:
      # Date format: https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: uploads/国家奖学金.jpg
          date_end: ''
          date_start: '2021-12-30'
          description: ''
          icon: ''
          organization: Ministry of Education of the People's Republic of China
          organization_url: ''
          title: National Scholarship
          url: ''
        - certificate_url: uploads/吴亚军专项奖学金.jpg
          date_end: ''
          date_start: '2022-12-30'
          description: ''
          icon: ''
          organization: Northwestern Polytechnical University
          organization_url: ''
          title: Yajun Wu Special Scholarship
          url: ''
        - certificate_url: uploads/小米优秀专项奖学金.jpg
          date_end: ''
          date_start: '2023-12-30'
          description: ''
          icon: ''
          organization: Northwestern Polytechnical University and Xiaomi Corporation
          organization_url: ''
          title: Xiaomi Excellent Scholarship
          url: ''
        - certificate_url: uploads/2021优秀大学生.jpg
          date_end: ''
          date_start: '2021-11-30'
          description: ''
          icon: ''
          organization: Northwestern Polytechnical University
          organization_url: ''
          title: 2021 Outstanding Student and First Class Scholarship
          url: ''
        - certificate_url: uploads/2022优秀大学生.jpg
          date_end: ''
          date_start: '2022-12-30'
          description: ''
          icon: ''
          organization: Northwestern Polytechnical University
          organization_url: ''
          title: 2022 Outstanding Student and First Class Scholarship
          url: ''
        - certificate_url: uploads/2023优秀大学生.jpg
          date_end: ''
          date_start: '2023-12-30'
          description: ''
          icon: ''
          organization: Northwestern Polytechnical University
          organization_url: ''
          title: 2023 Outstanding Student and First Class Scholarship
          url: ''
        - certificate_url: uploads/2024硕士一等学业奖学金.jpg
          date_end: ''
          date_start: '2024-10-30'
          description: ''
          icon: ''
          organization: University of Science and Technology of China
          organization_url: ''
          title: 2024 Master's First Class Scholarship
          url: ''
    design:
      columns: '2'
  - block: accomplishments
    content:
      title: 'Competition (Partial)'
      subtitle:
      date_format: Jan 2006
      items:
        - certificate_url: uploads/MCM.png
          date_end: ''
          date_start: '2023-12-30'
          description: ''
          icon: COMAP
          organization: The Consortium for Mathematics and Its Applications (COMAP)
          organization_url: https://www.comap.com/
          title: Mathematical Contest in Modeling (MCM) Finalist Award
          url: 'https://www.comap.com/contests/mcm-icm'
        - certificate_url: uploads/CUMCM.jpg
          date_end: ''
          date_start: '2022-12-30'
          description: ''
          icon: cumcm
          organization: China Society for Industrial and Applied Mathematics (CSIAM)
          organization_url: 'https://www.csiam.org.cn/'
          title: Contemporary Undergraduate Mathematical Contest in Modeling (CUMCM) Shaanxi First Award
          url: 'https://www.mcm.edu.cn/'
        - certificate_url: uploads/CUPT-Ind.jpg
          date_end: ''
          date_start: '2021-07-05'
          description: ''
          icon: CUPT
          organization: The Chinese Physical Society (CPS)
          organization_url: 'http://www.cps-net.org.cn/'
          title: China Undergraduate Physics Tournament (CUPT) Shaanxi Individual First Award
          url: 'https://www.cupt-iypt.com/'
        - certificate_url: uploads/CUPT-Team.jpg
          date_end: ''
          date_start: '2021-07-05'
          description: ''
          icon: CUPT
          organization: The Chinese Physical Society (CPS)
          organization_url: 'http://www.cps-net.org.cn/'
          title: China Undergraduate Physics Tournament (CUPT) Shaanxi Team First Award
          url: 'https://www.cupt-iypt.com/'
        - certificate_url: uploads/wenxin.jpg
          date_end: ''
          date_start: '2022-10-10'
          description: ''
          icon: wenxin
          organization: Baidu Wenxin
          organization_url: 'https://wenxin.baidu.com/'
          title: Baidu Wenxin LLM Application Co-construction GitHub A- Award
          url: 'https://wenxin.baidu.com/younger'
        - certificate_url: ''
          date_end: ''
          date_start: '2022-09-05'
          description: ''
          icon: nwpu
          organization: Northwestern Polytechnical University
          organization_url: 'https://en.nwpu.edu.cn/'
          title: Programming Competition First Award
          url: 'https://jiaowu.nwpu.edu.cn/info/1160/8306.htm'
        - certificate_url: uploads/math.jpg
          date_end: ''
          date_start: '2021-11-30'
          description: ''
          icon: nwpu
          organization: Northwestern Polytechnical University
          organization_url: 'https://en.nwpu.edu.cn/'
          title: Mathematics Competition First Award
          url: ''
        - certificate_url: uploads/physics.jpg
          date_end: ''
          date_start: '2021-05-30'
          description: ''
          icon: nwpu
          organization: Northwestern Polytechnical University
          organization_url: 'https://en.nwpu.edu.cn/'
          title: Physics Experiment Competition First Award
          url: 'https://physics.nwpu.edu.cn/info/1051/2013.htm'
    design:
      columns: '2'
  - block: accomplishments
    content:
      title: 'Other (Partial)'
      subtitle:
      date_format: Jan 2006
      items:
        - certificate_url: uploads/优秀毕业生.pdf
          date_end: ''
          date_start: '2024-06-30'
          description: ''
          icon: nwpu
          organization: Northwestern Polytechnical University
          organization_url: 'https://en.nwpu.edu.cn/'
          title: Outstanding Graduate
          url: 'https://mp.weixin.qq.com/s/9-KtgJ1bb4zE3UM3gUthdA'
        - certificate_url: uploads/CN116630684B.PDF
          date_end: ''
          date_start: '2025-04-01'
          description: 'A Lightweight End-to-End Object Segmentation Method for Road Damage Detection' 
          icon: zhuanli
          organization: China National Intellectual Property Administration
          organization_url: https://www.cnipa.gov.cn/
          title: Chinese Invention Patents
          url: 'https://pss-system.cponline.cnipa.gov.cn/conventionalSearch'
        - certificate_url: uploads/ASLP.jpg
          date_end: ''
          date_start: '2022-09-01'
          description: ''
          icon: aslp
          organization: Shaanxi Provincial Key Laboratory of Speech & Image Information Processing, ASLP@NPU Lab
          organization_url: https://www.cnipa.gov.cn/
          title: Excellent Intern in "AI Intelligent Speech Internship Program
          url: 'https://pss-system.cponline.cnipa.gov.cn/conventionalSearch'
        - certificate_url: uploads/十四运.jpg
          date_end: ''
          date_start: '2021-09-30'
          description: ''
          icon: shisiyun
          organization: General Administration of Sport
          organization_url: https://www.sport.gov.cn/n4/n23367606/index.html
          title: Flag phalanx member of the 14th National Games of the People's Republic of China
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
        - name: Deep Learning
          tag: Deep Learning
        - name: Other
          tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: markdown
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
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
        If you are interested, please contact me.
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
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/Twitter'
        - icon: skype
          icon_pack: fab
          name: Skype Me
          link: 'skype:echo123?call'
        - icon: video
          icon_pack: fas
          name: Zoom Me
          link: 'https://zoom.com'
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
