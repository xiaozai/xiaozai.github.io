---
title: "Anthropometric clothing measurements from 3D body scans"
collection: publications
permalink: /publications/2020-mva-anthropometry
venue: "Machine Vision and Applications (2020) 31, 7"
excerpt: 'Please check our Dataset : NOMO-3d-400-scans Dataset'
date: 2020-01-22
paperurl: https://doi.org/10.1007/s00138-019-01054-4
citation: 'Song Yan, Johan Wirta, Joni-Kristian Kämäräinen (2020). "Anthropometric clothing measurements from 3D body scans." <i>Machine Vision and Applications (2020)</i> 31, 7 '
---

## Abstract
We propose a full processing pipeline to acquire anthropometric measurements from 3D measurements. The first stage of our pipeline is a commercial point cloud scanner. In the second stage, a pre-defined body model is fitted to the captured point cloud. We have generated one male and one female model from the SMPL library. The fitting process is based on non-rigid Iterative Closest Point (ICP) algorithm that minimizes overall energy of point distance and local stiffness energy terms. In the third stage, we measure multiple circumference paths on the fitted model surface and use a non-linear regressor to provide the final estimates of anthropometric measurements. We scanned 194 male and 181 female subjects and the proposed pipeline provides mean absolute errors from 2.5 mm to 16.0 mm depending on the anthropometric measurement.

## Introduction
Anthropometric measurements, such as chest and hip circumference or shoulder-to-shoulder distance, provide detailed information about the body shape. The body shape information is essential for industrial design, clothing design, medical sciences and ergonomics. The measurements have traditionally been made manually from physical subject using a tape measure, but the raise of online shopping and personalized tools set new demand for computerized anthropometric measurements.

## Methods

3D Body scans 

SMPL Shape Model 

Mesh Registration 

Non-rigid ICP algorithm

SVR regressors.

## Results

The average fivefold errors for each anthropometric measurement and their accuracy thresholds and success rates are shown in Table 1. In all cases, the number of surface measurements were optimized for each anthropometric measurement and the best performing regressor (nonlinear SVR) was used. For the both male and female subjects the best performing measurement was neck circumference with 93% test cases below the threshold (6 mm) for men and 81% for women. The worst performing measure was ankle circumference for which only 28% of male 24% of female success rates were achieved. The error distributions for the male and female neck and ankle circumferences and male chest and female natural waist circumferences are shown in Fig. 6. The distributions reveal that there exists a small amount of test samples with a large error. It turned out that the main source of large estimation errors yields from the body scanner that often misses certain body parts. For example, feet regions often lack point cloud points which makes the registration fail in these regions (Fig. 7).

## Conclusion 

This work introduced a full processing pipeline for estimating physical anthropometric measurements from 3D body scans. The pipeline consisted of a commercial 3D scanner, a deformable SMPL body model, non-rigid ICP-based model registration, computation of circumference path features and nonlinear regression for anthropometric measurement estimation. Depending on the measurement, our pipeline provided success rates from 28% to 93% for male and from 24 to 82% for female subjects. The proposed pipeline works in practice and shows that an affordable scanning system can be built for clothing industry.

In the future work, we will further investigate and refine each step of the pipeline. For example, selection of better surface features in addition to the circumference paths, fast-to-compute alternatives for the slow ICP algorithm (e.g. Chen et al. [6]) and better scanners and scanning procedures.

## References
