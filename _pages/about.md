---
layout: about
title: about
permalink: /
subtitle: 

profile:
  align: left
  image: IMG_1463.jpeg
  image_circular: false # crops the image to make it circular
  

news: false # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false # includes social icons at the bottom of the page
---

Master's Student<br>
Department of Computer Science<br>
Stanford University<br>
Email: atharvac [at] cs [dot] stanford [dot] edu<br>
[Curriculum Vitae](/assets/pdf/CV_Oct_2026.pdf)<br>
[Google Scholar](https://scholar.google.com/citations?user=7oQ699AAAAAJ)<br>
[GitHub](https://github.com/atharva151101)<br>
<span style="color: var(--global-text-color-light);">Site last updated: {{ site.time | date: "%B, %Y" }}</span>

<div style="clear: both;"></div>

## About

I design programming systems and compilers that extract high performance from modern heterogeneous machines, at every scale from a single accelerator to an entire cluster. My goal is to develop programming abstractions, compiler techniques, and tools that account for the structure of these machines while making their performance accessible to programmers.

I am currently a Master's student in Computer Science at Stanford University, advised by [Fredrik Kjolstad](https://fredrikbk.com/). I received my B.Tech. in [Computer Science and Engineering](https://www.cse.iitm.ac.in/index.php) from the Indian Institute of Technology Madras, where I was advised by [Rupesh Nasre](https://cse.iitm.ac.in/~rupesh/) and [John Augustine](https://www.cse.iitm.ac.in/~augustine/index.html). I graduated at the top of my class at IITM and received the [B. Ravichandran Memorial Award](https://www.cse.iitm.ac.in/awards_details.php?arg=Mjk=) for this.

I interned on the ML Compute team at [Waymo](https://waymo.com/), where I worked on compiling JAX programs for Waymo's custom accelerators. Before Stanford, I was a Software Engineer on the Platform team at [Rubrik](https://www.rubrik.com/), where I worked on managing and scaling large-scale distributed systems. 

## Research

Modern computing systems are increasingly heterogeneous and hierarchical, combining different kinds of processors and memory at every scale from a single GPU to a large cluster. I design programming abstractions and compilers that map computations efficiently onto this structure, so programmers can get high performance without hand-tuning for each machine.

At Stanford, I work on sparse tensor compilers. Sparse computations are irregular and hence hard to parallelize. Together with [AJ Root](https://ajroot.pl/), I developed the first partitioning algorithm that provably load-balances any sparse tensor algebra expression across parallel execution units, and implemented it in Nacho, a compiler that automatically generates load-balanced kernels for parallel hardware (GPUs and multicore CPUs). This work will appear at [ASPLOS 2027](https://arxiv.org/abs/2604.17198). I am now building on Nacho to unify load balancing, vectorization, and tiling in sparse tensor compilers for GPUs.

At IIT Madras, for my undergraduate thesis, I worked on StarPlat, a domain-specific language for graph analytics whose compiler generates MPI, OpenMP, and CUDA code from high-level algorithm descriptions. I built StarPlat's distributed MPI backend and extended the language to support dynamic graphs, designing new primitives and a distributed representation for dynamic graphs. Before that, I have also worked on distributed systems theory, developing a new model of distributed computing and deriving its Byzantine fault tolerance properties.

## Publications
 

<div class="publications">
  {% bibliography --group_by none %}
</div>
