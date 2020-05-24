---
title: "Flash Lightens Gray Pixels"
collection: publications
permalink: /publications/2019-icip-flash
venue: "IEEE International Conference on Image Processing (ICIP2019)"
excerpt: ''
date: 2019-02-27
paperurl: https://arxiv.org/pdf/1902.10466.pdf
citation: 'Y Qian, S Yan, JK Kämäräinen, J Matas. "Anthropometric clothing measurements from 3D body scans." <i>IEEE International Conference on Image Processing (ICIP2019)</i> arXiv preprint arXiv:1902.10466 (2019) '
---

## Abstract
In the real world, a scene is usually cast by multiple illuminants and herein we address the problem of spatial illu- mination estimation. Our solution is based on detecting gray pixels with the help of flash photography. We show that flash photography significantly improves the performance of gray pixel detection without illuminant prior, training data or cali- bration of the flash. We also introduce a novel flash photography dataset generated from the MIT intrinsic dataset.

## Introduction
We address the illumination estimation problem which aims to measure the chroma of illumination in order to remove the color-bias from a captured image [1]. Illumination estima- tion can help in high-level vision tasks, e.g. object recogni- tion, tracking [2] and intrinsic image decomposition. There exists a large number of related works, from the traditional non-learning approaches [3] to recent deep learning based ap- proaches [4, 5, 6]. However, the vast majority of these works concentrate on the case of a single global illumination which is often an invalid assumption [7]. In this paper, we explore a more-complexless-optimisticsetting–mixedillumination


## Results
Results are summarized in Table 1 which shows the perfor- mance of flash gray pixel on the dataset in Section 4. “GP+f ” refers to flash gray pixel on the basis of the original gray pixel method “GP”. Results show that flash photography extensions of all gray pixel variants [13, 16, 17] systematically improve the results. For all three methods, the improvement over the whole dataset is over 40% in median and 30% in mean. The flash photography variants achieve the sufficient color con- stancy accuracy (≤ 3.0◦) in almost all cases. Fig. 3 illustrates predicted illumination between gray pixel methods and their flash variants. It is clear that the original versions cannot find the fine-grained details of mixed illumination. For example, the frog back and stomach are cast with different colors that confuses the original GP methods.

## Conclusion 
In this paper we reconsider gray pixel detection through the medium of flash photography. We find that computing a resid- ual map from the flash/no-flash pair, gray pixel methods can effectively measure the grayness of each pixel and provide spatial color constancy. We find that computing a residual map from the flash/no-flash pair, gray pixel methods can ef- fectively measure the grayness of each pixel, allowing a large margin improvement in spatially-varying illumination estimation. The method is pragmatic – it is lightweight, does not need any illuminant prior, training, flash light calibration or user input.

## References
