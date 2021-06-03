---
title: "Kinetics-TPS Challenge on Part-level Action Parsing"
excerpt: "Decomposing the action instance into a human part graph and detecting action labels for all human parts an as well the whole human. <br/><img src='/images/track3.gif'>"
collection: tracks
---

<img src='/images/track3_ori.gif' width="500" height="300">
{:.text-center}

**Track Organizers**: Xiao Ma, Ding Xia, Dongliang Wang, Weihao Gan, Junwei He 

Traditionally, action recognition has been treated as a high-level video classification problem. However, this manner ignores a detailed understanding of human actions. To fill this gap, we first develop a large-scale Kinetics-Temporal Part State (Kinetics-TPS) benchmark for this study. Kinetics-TPS provides part-level annotations in each video, which brings new opportunity to recognize a human action by compositional learning of body part state in videos.
{:.text-justify}

Different from existing video action datasets, our Kinetics-TPS provides 7.9M annotations of 10 body parts, 7.9M part state (i.e., how a body part moves) and 0.5M interactive objects in the video frames of 24 human action classes, which bring new opportunity to understand human action by compositional learning of body parts.
{:.text-justify}

The challenge aims at part state parsing for boosting action recognition in videos. To achieve this goal, we split the whole dataset as the train/test sets (3809/932 videos). In the training set, we provide all the ground truth annotations. In the test set, we only provide the test videos. For each test video, the task contains part state parsing in the frame level (including human instance localization, body part localization and part state recognition) and action recognition in the video level.
{:.text-justify}

The participants are required to provide two types of results. (1) Part State Parsing Result: For each frame in a test video, the participants should provide the predicted boxes of human instances, the predicted boxes of body parts as well as the predicted part state of each body part box. Note that, to reduce uploading burden, we will evaluate these results on the sampled frames of each test video (where the sampling interval is 5-frame). Hence, we encourage participants to provide the results on these frames. (2) Action Recognition Result: The participants should also provide the predicted action for each test video.
{:.text-justify}