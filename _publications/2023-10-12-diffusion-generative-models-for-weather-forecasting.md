---
title: "Diffusion generative models for weather forecasting"
collection: publications
category: thesis
status: published
permalink: /publication/2023-10-12-diffusion-generative-models-for-weather-forecasting
excerpt: 'This thesis is dedicated to investigating the application of diffusion models in the realm of weather forecasting, with a specific focus on precipitation nowcasting.'
date: 2023-10-12
venue: 'Università di Bologna, Corso di Studio in Informatica [LM-DM270]'
# slidesurl: ''
paperurl: 'https://amslaurea.unibo.it/id/eprint/29710/'
citation: 'Paparella, Alberto (2023) Diffusion generative models for weather forecasting. [Laurea magistrale], Università di Bologna, Corso di Studio in Informatica [LM-DM270].'
---

In recent years, traditional numerical methods used for accurate weather
prediction have faced increasing challenges from deep learning techniques.
The historical datasets commonly employed for short and medium-range
weather forecasts are typically structured in a regular spatial grid format.
This arrangement closely resembles images, with each weather variable akin
to a map or, when considering the temporal axis, as a video.
Several classes of generative models, including Generative Adversarial
Networks (GANs), Variational Autoencoders (VAEs), and the recent Denoising
Diffusion Models (DDMs), have demonstrated their effectiveness in
tackling the next-frame prediction problem. Consequently, it is only natural
to assess their performance in the context of weather prediction benchmarks.
DDMs, in particular, hold strong appeal in this domain due to the inherently
probabilistic nature of weather forecasting. This methodology aims to model
the probability distribution of weather indicators, with the expected value
representing the most likely prediction.
This thesis is dedicated to investigating the application of diffusion models
in the realm of weather forecasting, with a specific focus on precipitation
nowcasting. To achieve this, a specific subset of the ERA5 dataset has been
leveraged, encompassing hourly data for Western Europe spanning the years
2016 to 2021. Within this context, the effectiveness of diffusion models has
been rigorously assessed in the challenging domain of precipitation nowcasting.
The research is conducted in direct comparison to the well-established
U-Net models, as extensively documented in existing literature.
The proposed approach, referred to as Generative Ensemble Diffusion
(GED), harnesses a diffusion model to generate a diverse set of potential
weather scenarios. These scenarios are subsequently amalgamated into a
probable prediction through the application of a sophisticated post-processing
network. In direct contrast to recent deep learning models, the GED approach
consistently demonstrated superior performance across multiple performance
metrics, underscoring its significant advancement in the field of
weather forecasting.
