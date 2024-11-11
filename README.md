# CAMELYON+ BENCHMARK
## INTRODUCTION
### *why we do this work?*
Multiple Instance Learning **_(MIL)_** methods are mainstream approaches for pathological image classification and analysis.
The ***CAMELYON-16/17*** datasets are commonly used to evaluate ***MIL*** methods. 
However, they have the following issues:
* **_CAMELYON-16/17_** datasets contain some problematic slides
* Pixel-annotations of **_CAMELYON-16/17_** test-dataset not accurate enough
* Different **_MIL_** methods do not have a unified dataset-split and evaluation-metrics on the ***CAMELYON*** dataset
* To conclude,there is no ***BENCHMARK*** for ***MIL*** methods
### *what we do in this work?*
We do the following work to establish a ***CAMELYON+ BENCHMARK***
* Remove some problematic slides.
* Correct problematic annotations.
* Merge the correct version of**_CAMELYON-16/17_** datasets as the **_CAMELYON+_** dataset.
* Evaluate mainstream ***MIL*** methods on the **_CAMELYON-NEW_** dataset.
* Evaluate mainstream feature extractors on the **_CAMELYON-NEW_** dataset.
* Use more comprehensive evaluation metrics to assess different methods.
* In summary, we establish a new **_CAMELYON+ BENCHMARK_**.

## CAMELYON-NEW
### *balanced-dataset-split* 
* We apply balanced-dataset-split
* Details will be released soon
### *download*
* [BAIDU-PAN-LINK](https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md)
* [GOOGLE-PAN-LINK](https://github.com/lingxitong/CAMELYON_BENCHMARK/edit/main/README.md)
## BASELINE
* ***MEAN_MIL*** [Attention-based Deep Multiple Instance Learning](https://arxiv.org/abs/1802.04712) ***(ICML 2018)*** 
* ***MAX_MIL*** [Attention-based Deep Multiple Instance Learning](https://arxiv.org/abs/1802.04712) ***(ICML 2018)*** 
* ***AB_MIL*** [Attention-based Deep Multiple Instance Learning](https://arxiv.org/abs/1802.04712) ***(ICML 2018)*** 
* ***TRANS_MIL*** [Transformer based Correlated Multiple Instance Learning for WSI Classification](https://arxiv.org/abs/2106.00908) ***(NeurIPS 2021)***
* ***DS_MIL*** [Dual-stream MIL Network for WSI Classification with Self-supervised Contrastive Learning](https://arxiv.org/abs/2011.08939) ***(CVPR 2021)***
* ***CLAM_MIL*** [Data Efficient and Weakly Supervised Computational Pathology on WSI](https://arxiv.org/abs/2004.09666) ***(NAT BIOMED ENG 2021)***
* ***DTFD_MIL*** [Double-Tier Feature Distillation MIL for Histopathology WSI Classification](https://arxiv.org/abs/2203.12081) ***(CVPR 2022)***
* ***RRT_MIL*** [Towards Foundation Model-Level Performance in Computational Pathology](https://arxiv.org/abs/2402.17228) ***(CVPR 2024)***
* ***WIKG_MIL*** [Dynamic Graph Representation with Knowledge-aware Attention for WSI Analysis](https://arxiv.org/abs/2403.07719) ***(CVPR 2024)***
* ***UPDATING...***

## FEATURE-ENCODER
* ***VIT_S (IMAGENT-PRETRAINED)*** [Transformers for Image Recognition at Scale](https://arxiv.org/abs/2010.11929) ***(ICLR 2021)*** 
* ***PLIP (WSI-Contrastive-Learning)*** [A visual–language model for WSI using medical Twitter](https://www.nature.com/articles/s41591-023-02504-3) ***(NAT MED 2023)***
* ***UNI (WSI-PRETRAINED)*** [Towards a general-purpose foundation model for computational pathology](https://www.nature.com/articles/s41591-024-02857-3) ***(NAT MED 2024)***
* ***UPDATING...***

  
## SETTINGS
* Obtain the patches on 20X Magnification
* Keep the Hyperparameter settings of original implement
* Use uniform,balanced dataset-split


## RUSULTS
### REFINE-CAMELYON-17 (4 classes)
#### *VIT_S-METRICS*

|MIL|PARAMS|ACC|B-ACC|AUC|F1|PRE|
|:-----:|:-----:|:----:|:------:|:------:|:-------------:|:--------------:|
|MEAN|mobilenet|3.3M|34.02|10.56|60|60|
|MAX|mobilenet|3.3M|34.02|10.56|60|60|
|AB|mobilenet|3.3M|34.02|10.56|60|60|
|G-AB|mobilenet|3.3M|34.02|10.56|60|60|
|TRANS|mobilenet|3.3M|34.02|10.56|60|60|
|DS|mobilenet|3.3M|34.02|10.56|60|60|
|CLAM-SB|mobilenet|3.3M|34.02|10.56|60|60|
|CLAM_MB|mobilenet|3.3M|34.02|10.56|60|60|
|RRT|mobilenet|3.3M|34.02|10.56|60|60|
|WIKG|mobilenet|3.3M|34.02|10.56|60|60|

#### *PLIP-METRICS*

|MIL|PARAMS|ACC|B-ACC|AUC|F1|PRE|
|:-----:|:-----:|:----:|:------:|:------:|:-------------:|:--------------:|
|MEAN|mobilenet|3.3M|34.02|10.56|60|60|
|MAX|mobilenet|3.3M|34.02|10.56|60|60|
|AB|mobilenet|3.3M|34.02|10.56|60|60|
|G-AB|mobilenet|3.3M|34.02|10.56|60|60|
|TRANS|mobilenet|3.3M|34.02|10.56|60|60|
|DS|mobilenet|3.3M|34.02|10.56|60|60|
|CLAM-SB|mobilenet|3.3M|34.02|10.56|60|60|
|CLAM_MB|mobilenet|3.3M|34.02|10.56|60|60|
|RRT|mobilenet|3.3M|34.02|10.56|60|60|
|WIKG|mobilenet|3.3M|34.02|10.56|60|60|

#### *UNI-METRICS*

|MIL|PARAMS|ACC|B-ACC|AUC|F1|PRE|
|:-----:|:-----:|:----:|:------:|:------:|:-------------:|:--------------:|
|MEAN|mobilenet|3.3M|34.02|10.56|60|60|
|MAX|mobilenet|3.3M|34.02|10.56|60|60|
|AB|mobilenet|3.3M|34.02|10.56|60|60|
|G-AB|mobilenet|3.3M|34.02|10.56|60|60|
|TRANS|mobilenet|3.3M|34.02|10.56|60|60|
|DS|mobilenet|3.3M|34.02|10.56|60|60|
|CLAM-SB|mobilenet|3.3M|34.02|10.56|60|60|
|CLAM_MB|mobilenet|3.3M|34.02|10.56|60|60|
|RRT|mobilenet|3.3M|34.02|10.56|60|60|
|WIKG|mobilenet|3.3M|34.02|10.56|60|60|


#### *RESNET50-METRICS*

|MIL|PARAMS|ACC|B-ACC|AUC|F1|PRE|
|:-----:|:-----:|:----:|:------:|:------:|:-------------:|:--------------:|
|MEAN|mobilenet|3.3M|34.02|10.56|60|60|
|MAX|mobilenet|3.3M|34.02|10.56|60|60|
|AB|mobilenet|3.3M|34.02|10.56|60|60|
|G-AB|mobilenet|3.3M|34.02|10.56|60|60|
|TRANS|mobilenet|3.3M|34.02|10.56|60|60|
|DS|mobilenet|3.3M|34.02|10.56|60|60|
|CLAM-SB|mobilenet|3.3M|34.02|10.56|60|60|
|CLAM_MB|mobilenet|3.3M|34.02|10.56|60|60|
|RRT|mobilenet|3.3M|34.02|10.56|60|60|
|WIKG|mobilenet|3.3M|34.02|10.56|60|60|
