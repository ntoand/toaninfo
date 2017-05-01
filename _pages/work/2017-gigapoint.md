---
permalink: /work/2017-gigapoint
layout: work
title: Gigapoint - display large point datasets
keywords: pointcloud, potree
---

### **Platforms:** Linux, MacOS

### **Built with:** CMake, C++, Omegalib, OpenGL

Gigapoint is an <a href="https://github.com/uic-evl/omegalib" target="_blank">Omegalib</a> module to display large points datasets (e.g. LIDAR data) on desktop and visualisation cluster e.g. the CAVE2.

### **Features**

- Use <a href="http://potree.org/" target="_blank">potree</a> data as input
- Asynchronous and multi-threading file loading
- Support stereo display
- Eye Doom Lighting (EDL) filter
- Support live data update from a SLAM system
- Support data interaction with multiple wands e.g. track finding

![Century mine]({{ site.baseurl }}/assets/imgs/work/2017-gigapoint/02.jpg){: .image-center }
<p class="caption"><a href="https://en.wikipedia.org/wiki/Century_Mine" target="_blank">Century mine</a> (350 million points) dataset <sup>[1]</sup></p>

![Century mine surrouding dataset (750 million points)]({{ site.baseurl }}/assets/imgs/work/2017-gigapoint/03.jpg){: .image-center }
<p class="caption">Century mine surrouding dataset (750 million points) <sup>[1]</sup></p>

![Coloured by evelation with EDL filter]({{ site.baseurl }}/assets/imgs/work/2017-gigapoint/04.jpg){: .image-center }
<p class="caption">Coloured by evelation with EDL filter</p>

<div class="footnote"><a name="footnote1">1</a>:LIDAR data provided by Steve Micklethwaite to MIVP</div>
