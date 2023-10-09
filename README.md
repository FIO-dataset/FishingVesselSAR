# Introduction

This SAR fishing vessel dataset was created using 386 Chinese Gaofen-3 images, which contains 116 gillnetters, 72 seiners, and 181 trawlers. It contains images under multi-imaging mode, and different resolutions. And, all fishing vessel images were saved as single-precision floating-point amplitude SAR images. It can be utilized for studying the identification of fishing vessel types in SAR images.

The dataset's construction process is described in detail in the paper[ **Fishing Vessel Classification in SAR Images using a Novel Deep Learning Model**](https://ieeexplore.ieee.org/document/10242360), which is briefly described below:
1. For each SAR image, the corresponding AIS messages from the same zone were retrieved in a 10-minute window centered on the SAR acquisition time.

2. After performing the optimal spatiotemporal matches such as interpolation on AIS data, reliable links between AIS messages and the fishing vessels in SAR images were established. Then, we obtained SAR chips corresponding to 511 fishing vessels and their corresponding AIS data subject to strict quality control.

3. Based on AIS data, the fishing vessel identification model is used to reliably identify the fishing type of each SAR fishing vessel chip by comprehensively mining the differences that characterize different fishing vessel types. For detailed principles and the implementation process of the fishing vessel identification model, please refer to paper[ **Identification of Fishing Vessel Types and Analysis of Seasonal Activities in the Northern South China Sea Based on AIS Data: A Case Study of 2018**](https://www.mdpi.com/2072-4292/13/10/1952).

4. For the construction of the FishingVesselSAR dataset, the identification model identifies 511 fishing vessels as 116 gillnetters, 72 seiners, 181 trawlers, and 142 fishing vessels of uncertain type. Thus, the final FishingVesselSAR dataset contains SAR chips corresponding to 369 fishing vessels of known types.

## Cite as

**If you feel this dataset is useful, please cite as the following format.**

Y. Guan, X. Zhang, S. Chen, et al., "Fishing Vessel Classification in SAR Images using a Novel Deep Learning Model," in IEEE Transactions on Geoscience and Remote Sensing, doi: 10.1109/TGRS.2023.3312766.

## Contact

Copyright at the First Institute of Oceanography, Ministry of Natural Resources.
Please contact us if you have any questions: xi.zhang@fio.org.cn (Prof. Zhang).
