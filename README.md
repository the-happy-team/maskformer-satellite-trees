---
license: cc-by-nc-sa-4.0
tags:
- image-segmentation
widget:
- example_title: Manhattan
  src: https://i.imgur.com/Xhh8j1B.jpg
- example_title: Artshack
  src: https://i.imgur.com/zDQdmfr.jpg
- example_title: Cesario
  src: https://i.imgur.com/XLQKyf0.jpg
- example_title: Oakland
  src: https://i.imgur.com/buKTQvJ.jpg
datasets:
- thiagohersan/satellite-trees
---

Experimental model for segmenting vegetation on satellite images. And that is it. It just labels pixels as vegetation, other.

Created by finetuning the [facebook/maskformer-swin-base-ade model](https://huggingface.co/facebook/maskformer-swin-base-ade), and training with **a small number (~25)** of manually labeled satellite images of urban-ish areas.

## BIAS WARNING:
This model was created for a **personal** art and urbanism project and while the training set included images from geographically diverse cities of personal importance to me, it is in **no way exhaustive**. There are no cities in Asia, Africa, Central America or Oceania.

The urban areas included were of, or around, these cities:
- São Paulo
- Rio de Janeiro
- New York
- Pittsburgh
- Oakland
- Berlin
- Milan
- Riyadh

## EVALUATION WARNING:
**Anecdotally** speaking, it seems more precise than the original [facebook/maskformer-swin-base-ade model](https://huggingface.co/facebook/maskformer-swin-base-ade) model when used to get masks for vegetation.

It works with images of other cities, but success criteria is **qualitative**.