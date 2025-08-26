---
date:
  created: 2025-08-03
  updated: 2025-08-04
authors:
  - rappjer1
---

# AlphaEarth Foundation Satellite Embeddings

> “AlphaEarth Foundations provides a powerful new lens for understanding our planet by solving two major challenges: data overload and inconsistent information.” — from the “How AlphaEarth Foundations Works” section of the [DeepMind post](https://deepmind.google/discover/blog/alphaearth-foundations-helps-map-our-planet-in-unprecedented-detail/).

The key word is **lens**. That is what this product appears to be.

Before we look at the embeddings, let’s look at the spatial foundation used to build them. Here is a yearly Red, Green, and Blue composite from Sentinel-2 L1C that matches the 10 m resolution of the AEF embeddings.

![Sentinel-2 RGB composite of Michigan (2017)](./pics/glbasins_s2_glbasin_filled_mean_2017_blog.png)

This image is what most people imagine when they look at satellite data. It’s not far from a plane window view. When you first looked at it you likely noticed features relevant to your domain or places you know. Because of what _you know_, the image is worth more than its RGB components.

Now to the AEF satellite embeddings. They were produced by a model that sought to replicate that kind of understanding by digesting an individually incomprehensible volume of information and distilling it into vectors that capture small amounts of human-interpretable structure. When we visualize different embeddings as if they were the R, G, and B channels of a composite image, the results are fascinating because recognizable phenomena emerge.

However, with 64 unique embedding layers, checking every possible RGB combination (n = 41,664) would take time.

![Embeddings animation](./pics/glbasins_embeddings_filled_2017_labeled.gif)

The Earth Engine Developers site has solid [guides on using these embeddings for classic LULC and remote-sensing tasks](https://developers.google.com/earth-engine/tutorials/community/satellite-embedding-01-introduction). One clear use is similarity search and visual exploration, much like how people have used Google Earth, NAIP, and other high-resolution sources to curate training and validation datasets for models built on traditional EO inputs (e.g., Landsat and Sentinel).

A caution: do not treat these embeddings as if they were native sensor bands. EO instruments are chosen for known physical relationships to real-world processes. Embeddings are powerful, but they are still a black-box representation. As relationships to biomass, crop yield, and other variables are reported, we should ground them in the physics and measurements that trained the model. Foundation models should strengthen the case for continuing programs like Landsat and for expanding EO, ground validation, and basic science. The more **lenses** we have, the more complete our understanding of Earth’s condition and change.  

AI Disclaimer: Chatgpt/GPT-5 was used for editing this post and helping with generating some of the visualization pulled from Google Earth Engine. 

