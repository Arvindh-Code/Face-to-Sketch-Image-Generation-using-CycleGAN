# Face to Sketch Image Generation using CycleGAN

**Authors: Aravindh Gopalsamy, Abil Varkichan Jose**  
**Emails: gopal98aravindh@gmail.com, axv5324@mavs.uta.edu**

## Abstract

This project explores the use of CycleGAN for generating artistic sketches from face images. Leveraging the power of generative adversarial networks (GANs) in image-to-image translation, the primary goal is to transform realistic face images into expressive and artistic sketches. The CycleGAN model is trained on a dataset consisting of paired face images and corresponding sketches, allowing it to learn the mapping between the two domains. By incorporating cycle-consistency and adversarial loss functions, the model aims to capture essential facial features and translate them into visually appealing sketches while preserving identity and structural details. The project contributes to advancing image-to-image translation techniques with creative applications in digital art, design, and expression.

## Introduction

In the realm of computer vision, image-to-image translation has gained attention for its diverse applications in art, entertainment, and recognition. This project focuses on the unique challenge of generating artistic sketches from real face images. The proposed approach utilizes CycleGAN, a type of GAN suitable for unpaired image translation tasks. The significance lies in empowering digital artists and extending applications to law enforcement and forensic investigations.

## Dataset Description

The dataset combines the CUHK Face Sketch Database (CUFS) and the CUSK Dataset. CUFS includes 188 faces from the Chinese University of Hong Kong and others. The CUSK Dataset contributes 5000+ pairs, enhancing model accuracy. The dataset's uniformity, neutral expressions, and proper lighting facilitate high-quality sketch generation.


## Project Description

### Overview

The project implements a CycleGAN model for transforming facial photographs into expressive sketches. GANs, with a generator and discriminator, are trained competitively. CycleGAN, designed for unpaired data, introduces cycle-consistency loss for reversible translation. The model is trained on CUFS and CUSK datasets using adversarial, cycle-consistency, and identity loss functions.


### References

1. **Identity-Aware CycleGAN**: Introduces Identity-Aware Cycle GAN for face photo-sketch synthesis and recognition. Incorporates feedback training, various loss functions, and fine-tuning for identity preservation.

2. **Semi-supervised Cycle-GAN**: Proposes a semi-supervised learning framework for face photo-sketch translation. Introduces a pseudo-sketch feature and self-supervised training for improved generalization.

### Difference in Approach

The project differs by exclusively using upsampling/downsampling layers for image translation. The references focus on Identity-Aware paired data translation and semi-supervised learning. Due to limited face-sketch data, extensive preprocessing and optimized hyperparameters were crucial.


### Performance Comparison

The project optimizes epochs and hyperparameters, achieving improved face-sketch generation results (80% matching). Adversarial and cycle-consistency losses decrease, indicating enhanced translation quality. The model excels in capturing diverse artistic styles from photographs.


## Analysis

### Works Done and Strengths

- **Unpaired Image Translation**: Excels at learning the mapping between face photographs and sketches without paired data.
- **Cycle-Consistency Loss**: Preserves visual structure and content consistency, crucial for facial features and identity preservation.
- **Artistic Style Transfer**: Captures and transfers artistic styles from face photographs to sketches, enhancing creative potential.
- **Dataset Contribution**: CUFS and CUSK datasets provide a rich source for diverse facial features and sketch styles.

### Areas for Improvement

- **Cooperation for Diverse Data**: Collaboration with diverse data sources can enhance robustness and reduce bias.
- **Hyperparameter Tuning**: Fine-tuning hyperparameters and exploring new metrics for better generalization.
- **User-Centered Features**: Conducting user research, optimizing real-time applications, and enabling design processes.

### Future Work

- **Data Set Diversification**: Collaborate for diverse data sets to capture more facial features and artistic styles.
- **User-Centered Design**: Conduct user research for better user-oriented features and applications.
- **Real-Time Optimization**: Optimize for real-time applications and evaluate conditional generation.

## Conclusion

The CycleGAN implementation for face-sketch conversion represents a significant advancement in image translation. Its ability to generate expressive and diverse sketches from face photographs holds promise for digital art, design, and entertainment applications. While the project demonstrates industry-standard results, ongoing work includes diversifying datasets, fine-tuning hyperparameters, and exploring user-centered features. This work contributes to the growing field of image-to-image translation and emphasizes the role of GANs in pushing the boundaries of creative expression.

## References

1. [Identity-Aware CycleGAN for Face Photo-Sketch Synthesis and Recognition](https://arxiv.org/pdf/2103.16019.pdf)
2. [Semi-supervised Cycle-GAN for Face Photo-Sketch Translation in the Wild](https://arxiv.org/pdf/2307.10281.pdf)
3. [Landmark Assisted CycleGAN for Cartoon Face](https://arxiv.org/pdf/1907.01424.pdf)

Dataset Credits: [CUHK Face Sketch Database (CUFS)](https://mmlab.ie.cuhk.edu.hk/archive/CUFS/)
  
[Jun-Yan Zhu, et al. "Unpaired Image-to-Image Translation Using Cycle-Consistent Adversarial Networks." ICCV 2017.](https://arxiv.org/abs/1703.10593)

[Ming-Yu Liu, et al. "Unsupervised Image-to-Image Translation Networks." NeurIPS 2017.](https://arxiv.org/abs/1701.02676)
