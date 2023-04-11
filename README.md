# Image to Prompt

## Motivation and Background

[Stable Diffusion - Image to Prompts](https://www.kaggle.com/competitions/stable-diffusion-image-to-prompts/overview) is a competition on Kaggle.

The goal of this competition is to reverse the typical direction of a generative text-to-image model: instead of generating an image from a text prompt.

We want to  create a model which can predict the text prompt given a generated image. And making predictions on a dataset containing a wide variety of $\verb|(prompt, image)|$ pairs generated by Stable Diffusion 2.0, in order to understand how reversible the latent relationship is.

## Methodology


## Application and Datasets

### Application

Based on the Kaggle competition, we want to build a model to predict the prompts that were used to generate target images.

### Datasets

Prompts for this challenge were generated using a variety of (non disclosed) methods, and range from fairly simple to fairly complex with multiple objects and modifiers.

Images were generated from the prompts using Stable Diffusion $2.0$ ($768$-v-ema.ckpt) and were generated with 50 steps at $768 \times 768$ px and then downsized to $512 \times 512$ for the competition dataset. The hidden re-run test folder contains approximately $16,000$ images.

## References

[1] [Learning Transferable Visual Models From Natural Language Supervision](https://arxiv.org/pdf/2103.00020.pdf)

[2] [An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale](https://arxiv.org/pdf/2010.11929.pdf)

[3] [Very Deep Convolutional Networks for Large-Scale Image Recognition](https://arxiv.org/pdf/1409.1556.pdf)

[4] [SentenceTransformers](https://www.sbert.net/)

[5] [CLIPInterrogator + OFA + ViT](https://www.kaggle.com/code/motono0223/clipinterrogator-ofa-vit)

[
