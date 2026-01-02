---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
profile:
  align: right
  image: prof_pic.jpg
---

<!-- ![image](assets/peacock.jpg){: style="float: right"; height="25%" width="25%"} -->

\[[CV](https://raw.githubusercontent.com/LedgeDash/ledgedash.github.io/main/assets/files/cv-davidliu.pdf) \| [LinkedIn](https://www.linkedin.com/in/david-hao-liu-160307/) \| [GitHub](https://github.com/LedgeDash) \| [Google Scholar](https://scholar.google.com/citations?user=Mg4erJ8AAAAJ&hl=en)\]

I'm a software engineer at Google working on systems for LLM performance tuning and eval.

I'm broadly interested in systems. My graduate school research focused on serverless computing problems such as orchestrating large-scale
serverless applications and speeding up lightweight virtual machines.
Previously, I worked on information flow control, first for the Android and
later for IoT applications. Even earlier I worked on Linux kernel drivers for storage
servers when I occasionally debugged by looking at how the LEDs on the
motherboard lit up.

# Work Experience

**Google**, Senior Software Engineer, since 2024.1

* _GenAI Systems, Google Deepmind_ (2025-)
* _TPU Performance_ (2024-2025)
  * XLA compiler auto-optimization
  * Systems for ML performance optimization
  * LLM post training

**Nimble Storage**, Member of Technical Staff, 2015 - 2017
* Linux kernel driver developer for storage servers

# Education

**Princeton University**, 2017 - 2023
* Ph.D. in Computer Science
* Dissertation: [A Serverless Architecture for Application-Level Orchestration](https://dataspace.princeton.edu/handle/88435/dsp017w62fc456)
* Advisor: [Prof. Amit Levy](https://www.amitlevy.com/)

**Duke University**, 2011 - 2015
* B.S.E in Electrical and Computer Engineering, minor in mathematics

# Papers

{%- assign publications = site.data.publications | sort: "year" | reverse -%}
{% for publication in publications %}

* __{{ publication.title }}__  
   {{ publication.authors }}  
   _{{ publication.venue }}_  
   {% if publication.abbr %} {{ publication.abbr }}  
   {% if publication.paper %}\[[paper]({{ publication.paper }})\]{% endif %}
   {% if publication.slides %}\[[slides]({{ publication.slides }})\]{%- endif -%}
   {% if publication.poster %}\[[poster]({{ publication.poster }})\]{% endif %}
   {% if publication.code%}\[[code]({{ publication.code}})\]{% endif %}
   {% if publication.video%}\[[video]({{ publication.video}})\]{% endif %}
   {%- else -%}
   {% if publication.paper %}\[[paper]({{ publication.paper }})\]{% endif %}
   {% if publication.slides %}\[[slides]({{ publication.slides }})\]{%- endif -%}
   {% if publication.poster %}\[[poster]({{ publication.poster }})\]{% endif %}
   {% if publication.code%}\[[code]({{ publication.code}})\]{% endif %}
   {% endif %}

{% endfor %}

