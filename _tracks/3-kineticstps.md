---
title: "Kinetics-TPS Challenge on Part-level Action Parsing"
excerpt: "Decomposing the action instance into a human part graph and detecting action labels for all human parts an as well the whole human. <br/><img src='/images/500x300.png'>"
collection: tracks
---

<img src='/images/500x300.png'>

**Track Organizers**: Dongliang Wang, Weihao Gan, Xiao Ma, Ding Xia 

Traditionally, action recognition has been treated as a high-level video classification problem. However, this manner ignores a detailed understanding of human actions. To fill this gap, we first develop a large-scale Kinetics-TPS (Temporal Part State) benchmark for this study. Kinetics-TPS provides spatio-temporal part-level action graph annotations for videos from a subset of Kinetics Motion[10] dataset, which brings new opportunity to recognize a human action by compositional learning of body part state in videos.

Kinetics-TPS provides millions of annotations for 913K frames of 5833 videos from a subset of Kinetics Motion (30 action class). The annotations include 1.9 M human bounding box, 0.7 M objects bounding box of 230 class, 9.5 M bounding boxes of 10 body parts classes, and 8.6 M (part, part state, object) tuple annotation of 71 part-level verbs classes.

The track aims at part-level action parsing for action videos and boosting action recognition performance with this detailed action understanding information. There are two different subtasks for this track resulting from whether the ground truth bounding box location of objects and human body parts and their categories. However, both subtasks expect to output a detailed part-level action graph and the video action classification result with the help of this parsed graph. Both subtasks are carried out on our official train and test split of the Kinetics- TPS dataset.