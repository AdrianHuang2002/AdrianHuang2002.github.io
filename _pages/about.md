---
layout: about
title: about
permalink: /
subtitle: University of Massachusetts Amherst

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false
  more_info: >
    <p>740 N Pleasant St</p>
    <p>Amherst, MA 01003</p>

# Page widgets
selected_papers: false   # shows selected publications list if true
social: true             # social icons footer

# Optional widgets below (left disabled)
announcements:
  enabled: false
  scrollable: true
  limit: 5

latest_posts:
  enabled: false
  scrollable: true
  limit: 3
---

I’m a first-year M.S. student in Computer Science at UMass Amherst, where I work with the
[Embodied AGI Group](https://embodied-agi.cs.umass.edu/people/) led by
[Chuang Gan](https://people.csail.mit.edu/ganchuang/).
Previously, I was part of the UMD [Gamma Group](https://gamma.umd.edu/) mentored by
[Xijun Wang](https://xijun-cs.github.io/) and under the guidance of
[Dinesh Manocha](https://www.cs.umd.edu/people/dmanocha). I’ve also collaborated with
[John P. Dickerson](https://jpdickerson.com/) in the Dickerson Lab.

My current research interests are primarily centered on **humanoid robots**.

## 📚 Publications
{% include selected_papers.liquid %}

## 💼 Experience
{% assign exp = site.data.cv | where: "title", "Experience" | first %}
{% if exp %}
  {% include cv/experience.liquid items=exp.contents %}
{% endif %}

## 🎓 Education
{% assign edu = site.data.cv | where: "title", "Education" | first %}
{% if edu %}
  {% include cv/experience.liquid items=edu.contents %}
{% endif %}


