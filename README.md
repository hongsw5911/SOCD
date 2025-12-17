# SOCD
This repository is the official implementation of “How Can We Mitigate Object Hallucination In Real World? Make Divergent Logits With Contrastive Tokens”

# Abstract
How can we minimize object hallucination in responses that Large Vision-Language Models (LVLMs) autoregressively generate in visually uncertain scenes? Object Hallucination (OH) refers to the phenomenon where LVLMs generate responses containing objects that are not present in the given image. This issue is exacerbated in real-world settings, where LVLMs not only generate responses autoregressively but also encounter scenes with increased visual uncertainty due to factors such as a large number of objects, occlusion, and motion blur. Ensuring that LVLMs do not commit OH under such conditions is a prerequisite for their reliable and widespread deployment in real-world applications. Despite recent progress, the effectiveness of existing de-hallucination methods under these real-world conditions remains largely unexplored.

In this work, (i) we show that existing de-hallucination methods fail to reduce object hallucination throughout autoregressive generation, (ii) we introduce PracticeOH, a benchmark designed to evaluate de-hallucination performance under visually uncertain scenes, and (iii) we propose SOCD (Semantically Opposing Contrastive Decoding), a training-free de-hallucination method that mitigates object hallucination not only during autoregressive generation but also under visually uncertain conditions. Experimental results demonstrate that SOCD achieves up to a 15.5% error-rate reduction over baseline methods, even when generating responses in visually uncertain real-world scenarios.
# Datasets

We use the following datasets to evaluate SOCD.

| Dataset | Type | Source |
|--------|------|--------|
| **MSCOCO** | Real-world | <https://cocodataset.org/#home> |
| **Objects365** | Real-world | <https://www.objects365.org/overview.html> |
| **Cityscapes** | Real-world | <https://www.cityscapes-dataset.com/> |
