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

I recently completed my Ph.D. in Computer Science at Princeton Univerisity
where I was a member of the
[Princeton Network Systems (SNS) group](https://sns.cs.princeton.edu/).
Previously, I received my B.S.E. in Electrical and Computer Engineering and a minor in
Mathematics from Duke University.

I am broadly interested in systems, with about 8 years of experience in software development.
My most recent research focuses on serverless computing problems such as orchestrating large-scale
serverless applications and speeding up lightweight virtual machines.
Previously, I worked on information flow control, first for the Android operating system and
later for IoT applications. Even earlier I worked on Linux kernel drivers for storage
servers when I occasionally debugged by looking at how the LEDs on the
motherboard lit up.

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


# Personal

When I'm not working on a computer, I enjoy music, singing, gardening, and
playing a few rounds of board games with friends and family. My [wife](https://www.smu.edu/cox/Our-People-and-Community/Faculty/Rowena-J-Gan) and I currently live in Dallas.
