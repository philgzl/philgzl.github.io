---
layout: page
title: Philippe Gonzalez
---

# About me

I am a postdoctoral researcher at the Hearing Systems section at the Technical University of Denmark. I wrote my PhD thesis on deep learning-based speech enhancement from 2020 to 2023 at the Technical University of Denmark under the supervision of Tobias May and Tommy Sonne Alstrøm. My research interests include audio signal processing, deep learning-based speech enhancement and source separation, the generalization of learning-based systems, and model-based hearing loss compensation.

As a kid, I grew up in Colombia, Ivory Coast, Turkey, and Peru. I can speak English, French, Spanish, and some Danish. I play the bass in band, collect vinyl records, and occasionally DJ at parties. I like playing video games, especially Dota 2 in which I am a highly ranked player. Other hobbies include tennis, electronics, photography, and chess. I love dogs.

# Publications

## <a href="https://doi.org/10.48550/arXiv.2406.06160">The Effect of Training Dataset Size on Discriminative and Diffusion-Based Speech Enhancement Systems</a>

Philippe Gonzalez, Zheng-Hua Tan, Jan Østergaard, Jesper Jensen, Tommy Sonne Alstrøm, and Tobias May.

In review. <a href="/lst">Audio examples</a>.

<p class=abstract>Abstract: The performance of deep neural network-based speech enhancement systems typically increases with the training dataset size. However, studies that investigated the effect of training dataset size on speech enhancement performance did not consider recent approaches, such as diffusion-based generative models. Diffusion models are typically trained with massive datasets for image generation tasks, but whether this is also required for speech enhancement is unknown. Moreover, studies that investigated the effect of training dataset size did not control for the data diversity. It is thus unclear whether the performance improvement was due to the increased dataset size or diversity. Therefore, we systematically investigate the effect of training dataset size on the performance of popular state-of-the-art discriminative and diffusion-based speech enhancement systems. We control for the data diversity by using a fixed set of speech utterances, noise segments and binaural room impulse responses to generate datasets of different sizes. We find that the diffusion-based systems do not benefit from increasing the training dataset size as much as the discriminative systems. They perform the best relative to the discriminative systems with datasets of 10 h or less, but they are outperformed by the discriminative systems with datasets of 100 h or more.</p>

## <a href="https://doi.org/10.48550/arXiv.2312.04370">Investigating the Design Space of Diffusion Models for Speech Enhancement</a>

Philippe Gonzalez, Zheng-Hua Tan, Jan Østergaard, Jesper Jensen, Tommy Sonne Alstrøm, and Tobias May.

In review.

<p class=abstract>Abstract: Diffusion models are a new class of generative models that have shown outstanding performance in image generation literature. As a consequence, studies have attempted to apply diffusion models to other tasks, such as speech enhancement. A popular approach in adapting diffusion models to speech enhancement consists in modelling a progressive transformation between the clean and noisy speech signals. However, one popular diffusion model framework previously laid in image generation literature did not account for such a transformation towards the system input, which prevents from relating the existing diffusion-based speech enhancement systems with the aforementioned diffusion model framework. To address this, we extend this framework to account for the progressive transformation between the clean and noisy speech signals. This allows us to apply recent developments from image generation literature, and to systematically investigate design aspects of diffusion models that remain largely unexplored for speech enhancement, such as the neural network preconditioning, the training loss weighting, the stochastic differential equation (SDE), or the amount of stochasticity injected in the reverse process. We show that the performance of previous diffusion-based speech enhancement systems cannot be attributed to the progressive transformation between the clean and noisy speech signals. Moreover, we show that a proper choice of preconditioning, training loss weighting, SDE and sampler allows to outperform a popular diffusion-based speech enhancement system in terms of perceptual metrics while using fewer sampling steps, thus reducing the computational cost by a factor of four.</p>

## <a href="https://doi.org/10.48550/arXiv.2312.02683">Diffusion-Based Speech Enhancement in Matched and Mismatched Conditions Using a Heun-Based Sampler</a>

Philippe Gonzalez, Zheng-Hua Tan, Jan Østergaard, Jesper Jensen, Tommy Sonne Alstrøm, and Tobias May.

IEEE International Conference on Acoustics, Speech, and Signal Processing, 2024.

<p class=abstract>Abstract: Diffusion models are a new class of generative models that have recently been applied to speech enhancement successfully. Previous works have demonstrated their superior performance in mismatched conditions compared to state-of-the art discriminative models. However, this was investigated with a single database for training and another one for testing, which makes the results highly dependent on the particular databases. Moreover, recent developments from the image generation literature remain largely unexplored for speech enhancement. These include several design aspects of diffusion models, such as the noise schedule or the reverse sampler. In this work, we systematically assess the generalization performance of a diffusion-based speech enhancement model by using multiple speech, noise and binaural room impulse response (BRIR) databases to simulate mismatched acoustic conditions. We also experiment with a noise schedule and a sampler that have not been applied to speech enhancement before. We show that the proposed system substantially benefits from using multiple databases for training, and achieves superior performance compared to state-of-the-art discriminative models in both matched and mismatched conditions. We also show that a Heun-based sampler achieves superior performance at a smaller computational cost compared to a sampler commonly used for speech enhancement.</p>

## <a href="https://doi.org/10.1109/TASLP.2023.3318965">Assessing the Generalization Gap of Learning-Based Speech Enhancement Systems in Noisy and Reverberant Environments</a>

Philippe Gonzalez, Tommy Sonne Alstrøm, and Tobias May.

IEEE/ACM Transactions on Audio, Speech, and Language Processing, 2023.

<p class=abstract>Abstract: The acoustic variability of noisy and reverberant speech mixtures is influenced by multiple factors, such as the spectro-temporal characteristics of the target speaker and the interfering noise, the signal-to-noise ratio (SNR) and the room characteristics. This large variability poses a major challenge for learning-based speech enhancement systems, since a mismatch between the training and testing conditions can substantially reduce the performance of the system. Generalization to unseen conditions is typically assessed by testing the system with a new speech, noise or binaural room impulse response (BRIR) database different from the one used during training. However, the difficulty of the speech enhancement task can change across databases, which can substantially influence the results. The present study introduces a generalization assessment framework that uses a reference model trained on the test condition, such that it can be used as a proxy for the difficulty of the test condition. This allows to disentangle the effect of the change in task difficulty from the effect of dealing with new data, and thus to define a new measure of generalization performance termed the generalization gap. The procedure is repeated in a cross-validation fashion by cycling through multiple speech, noise, and BRIR databases to accurately estimate the generalization gap. The proposed framework is applied to evaluate the generalization potential of a feedforward neural network (FFNN), Conv-TasNet, DCCRN and MANNER. We find that for all models, the performance degrades the most in speech mismatches, while good noise and room generalization can be achieved by training on multiple databases. Moreover, while recent models show higher performance in matched conditions, their performance substantially decreases in mismatched conditions and can become inferior to that of the FFNN-based system.</p>

## <a href="https://doi.org/10.1109/ICASSP49357.2023.10097075">On Batching Variable Size Inputs for Training End-to-End Speech Enhancement Systems</a>

Philippe Gonzalez, Tommy Sonne Alstrøm, and Tobias May.

IEEE International Conference on Acoustics, Speech, and Signal Processing, 2023.

<p class=abstract>Abstract: The performance of neural network-based speech enhancement systems is primarily influenced by the model architecture, whereas training times and computational resource utilization are primarily affected by training parameters such as the batch size. Since noisy and reverberant speech mixtures can have different duration, a batching strategy is required to handle variable size inputs during training, in particular for state-of-the-art end-to-end systems. Such strategies usually strive for a compromise between zero-padding and data randomization, and can be combined with a dynamic batch size for a more consistent amount of data in each batch. However, the effect of these strategies on resource utilization and more importantly network performance is not well documented. This paper systematically investigates the effect of different batching strategies and batch sizes on the training statistics and speech enhancement performance of a Conv-TasNet, evaluated in both matched and mismatched conditions. We find that using a small batch size during training improves performance in both conditions for all batching strategies. Moreover, using sorted or bucket batching with a dynamic batch size allows for reduced training time and GPU memory usage while achieving similar performance compared to random batching with a fixed batch size.</p>
