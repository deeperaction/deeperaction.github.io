---
title: "MultiSports Challenge on Spatio-Temporal Action Detection"
excerpt: "Localizing all action instances with spatio-temporal tubes and recognizing their labels from untrimmed and multi-person videos.  <br/><img src='/images/sports.gif'>"
collection: tracks
---

<img src='/images/sports_ori.gif' width="500" height="300">
{:.text-center}

**Track Organizers**: Yixuan Li, Lei Chen, Runyu He, Zhenzhi Wang

Spatio-temporal action localization is an important and challenging problem in video understanding. Current spatio-temporal action localization benchmarks can be mainly classified into two categories: 1) Densely annotated high-level actions such as J-HMDB and UCF101-24, but their video clips typically only have a single person doing some semantically simple and temporally repeated actions. 2) Sparsely annotated actions such as AVA and DALY that fail to provide clear temporal action boundaries, and thus might be unsuitable for modeling actions with fast movement, and temporal evolution.
{:.text-justify}

To facilitate the study of spatio-temporal action localization, we develop MultiSports, short for Multi-person Sports Actions. The dataset is large-scale, high-quality and contains 25fps frame- by-frame annotations of multi-person action labels with precise temporal boundaries. The action vocabulary consists of 66 action labels collected from 4 sports (basketball, volleyball, football and aerobic gymnastics), all of which are defined by either professional athletes or official documentations. Meanwhile, the advantage of sports actions also lies in the complex human-object-scene interactions compared with atomic actions. In football, for example, although the athlete only takes 0.5s to kick the ball, we may need up to 5s' context to understand whether it is short pass, long pass, through pass or cross. Likewise, when faced with the similar motions of shooting in basketball, the position of the athlete becomes critical for determining whether it is a 2-point shot or a 3-point shot. Finally, the multi-person sports actions reveals more realistic challenges of spatio-temporal action detection, such as fast movement, large deformation of actors, action occlusion and small size of both humans and objects.
{:.text-justify}

Following AVA, we evaluate on 60 classes which have at least 25 instances in validation and test splits to benchmark performance. Following the standard practice of UCF dataset, we utilize frame mAP and video mAP to evaluate action localization performance. For video map, we use the 3D IoU, which is defined as the temporal domain IoU of two tracks, multiplied by the average of the IoU between the overlapping frames. The threshold is 0.5 for frame-mAP, 0.2 and 0.5 for video-mAP.
{:.text-justify}