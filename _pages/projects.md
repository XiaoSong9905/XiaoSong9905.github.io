---
layout: archive
title: "Project"
permalink: /projects/
author_profile: true
redirect_from:
  - /projects
  - /projects.html
---

{% include base_path %}

DGEMM on Cori KNL Node (C++, AVX2, AVX512)
------
[Link to github repo](https://github.com/XiaoSong9905/dgemm-knl)
* Implement DGEMM on Intel Cori Node. Achieve average of 75% MKL performance on single core.
* Use AVX512 inline assembly for embedded broadcast, increase theoratical peak from 22.4 to 44.8 GFLOPs.
* Mix use of AVX2 & AVX512 for 8x8 matrix transpose, reduce the pressure on load port. Incr 0.4% peak perf.




Search Engine from Scratch (C++)
------
* Mainly responsible for search engine back-end: webpage crawler and HTML parser.
* Implement our STL string, vector, map, priority queue.
* Use pthread, OpenSSL, and socket to implement multi-machine multi-thread crawler that supports download prioritized web pages, remove duplicated web pages, handling URL redirection, and support IPv4 & IPv6 download at the same time.
* Implement HTML parser to extract URL links, anchor text, title, and body from HTML. Our parser can handle more corner cases than Python 3 html.parser.