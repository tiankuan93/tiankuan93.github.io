---
title: "Towards Real-Time Neural Video Codec for Cross-Platform Application Using Calibration Information"
collection: publications
permalink: /publication/2023-10-01-towards-realtime-video-codec/
date: 2023-10-01
venue: 'Arxiv'
paperurl: 'https://browse.arxiv.org/pdf/2309.11276.pdf'
citation: 'Kuan Tian, Yonghang Guan, Jinxi Xiang, Jun Zhang, et. al'
---

<a href='https://arxiv.org/abs/2309.11276'>Paper is here</a>

## Abstract

The state-of-the-art neural video codecs have outperformed the most sophisticated traditional codecs in terms of RD performance in certain cases. However, utilizing them for practical applications is still challenging for two major reasons. 1) Cross-platform computational errors resulting from floating point operations can lead to inaccurate decoding of the bitstream. 2) The high computational complexity of the encoding and decoding process poses a challenge in achieving real-time performance. In this paper, we propose a real-time cross-platform neural video codec, which is capable of efficiently decoding of 720P video bitstream from other encoding platforms on a consumer-grade GPU. First, to solve the problem of inconsistency of codec caused by the uncertainty of floating point calculations across platforms, we design a calibration transmitting system to guarantee the consistent quantization of entropy parameters between the encoding and decoding stages. The parameters that may have transboundary quantization between encoding and decoding are identified in the encoding stage, and their coordinates will be delivered by auxiliary transmitted bitstream. By doing so, these inconsistent parameters can be processed properly in the decoding stage. Furthermore, to reduce the bitrate of the auxiliary bitstream, we rectify the distribution of entropy parameters using a piecewise Gaussian constraint. Second, to match the computational limitations on the decoding side for real-time video codec, we design a lightweight model. A series of efficiency techniques enable our model to achieve 25 FPS decoding speed on NVIDIA RTX 2080 GPU. Experimental results demonstrate that our model can achieve real-time decoding of 720P videos while encoding on another platform. Furthermore, the real-time model brings up to a maximum of 24.2% BD-rate improvement from the perspective of PSNR with the anchor H.265.