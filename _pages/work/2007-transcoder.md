---
permalink: /work/2007-transcoder
layout: work
title: MPEG-4 to H.264 transcoder
keywords: transcoder, MPEG-4, H.264, video
---

### **Platforms:** Windows

### **Built with:** C++, Visual Studio C++

Efficient downscaling in a transcoder is important when the output should be converted to a lower resolution video. In this work, I suggest a fast spatial downscaling method for transcoding video from MPEG-4 SP (with Simple Profile) to H.264. Based on frame image characteristics and motion information in MPEG-4 decoder, I limit motion modes, generate prediction motion vectors and build an adaptive search range for motion estimation in H.264 encoder. Simulation results show that the transcoder considerably reduces transcoding time while video quality is kept almost optimal.

The transcoder converts MPEG-4 Simple Profile bitstream to H.264 Main Profile bitstream. Notice:
- The MPEG-4 bitstream must be encoded in Simple Profile
- The transcoder not using Rate Distortion Optimization

![Transcoder diagram]({{ site.baseurl }}/assets/imgs/work/2007-transcoder/02.jpg){: .image-center }
<p class="caption">Transcoder diagram</p>

In this architecture the input MPEG-4 bitstream is decoded by MPEG-4 decoder. The transcoder decodes and encodes frame by frame. After decoding one frame, the frame data is transferred to H.264 encoder as input frame and the motion estimation is reused to reduce encoding time. Because the motion compensation module in H.264 encoder accounts 60-70% of total cost, reusing motion information from MPEG-4 decoder significantly reduces encode time.

![Some results]({{ site.baseurl }}/assets/imgs/work/2007-transcoder/03.jpg){: .image-center }
<p class="caption">Some results</p>
