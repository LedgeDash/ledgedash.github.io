---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
profile:
  align: right
  image: prof_pic.jpg
---

<!-- ![image](assets/peacock.jpg){: style="float: right"; height="25%" width="25%"} -->

\[[CV](https://raw.githubusercontent.com/LedgeDash/ledgedash.github.io/main/assets/files/cv.pdf) \| [GitHub](https://github.com/LedgeDash) \| [Google Scholar](https://scholar.google.com/citations?user=Mg4erJ8AAAAJ&hl=en)\]

I am a PhD student at Princeton University in Computer Science, advised by
[Amit Levy](https://www.amitlevy.com/). I am a member of the [Princeton S\*
Network Systems (SNS) group](https://sns.cs.princeton.edu/). Previously, I
received a B.S. in Electrical and Computer Engineering and a minor in
Mathematics from Duke University.

I am broadly interested in systems and security. My most recent research
focuses on serverless computing problems such as orchestrating large-scale
serverless applications and speeding up lightweight virtual machines. Before
that, I worked on IFC and taint tracking, first for Android apps and later for
IoT apps.


# Papers

{%- assign publications = site.data.publications | sort: "year" | reverse -%}
{% for publication in publications %}

* __{{ publication.title }}__  
   {{ publication.authors }}  
   _{{ publication.venue }}_  
   {% if publication.abbr %} {{ publication.abbr }}  
   {% if publication.paper %}\[[paper]({{ publication.paper }})\]{% endif %}
   {% if publication.presentation %}\[[presentation]({{ publication.presentation }})\]{%- endif -%}
   {% if publication.poster %}\[[poster]({{ publication.poster }})\]{% endif %}
   {% if publication.code%}\[[code]({{ publication.code}})\]{% endif %}
   {%- else -%}
   {% if publication.paper %}\[[paper]({{ publication.paper }})\]{% endif %}
   {% if publication.presentation %}\[[presentation]({{ publication.presentation }})\]{%- endif -%}
   {% if publication.poster %}\[[poster]({{ publication.poster }})\]{% endif %}
   {% if publication.code%}\[[code]({{ publication.code}})\]{% endif %}
   {% endif %}

{% endfor %}


# Personal

When I'm not working on a computer, I enjoy music, singing, gardening, and
playing a few rounds of board games with friends and family.
