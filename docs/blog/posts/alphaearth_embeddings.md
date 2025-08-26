---
date:
  created: 2025-08-03
  updated: 2025-08-04
authors:
  - rappjer1
---

# AlphaEarth Foundation Satellite Embeddings 


“AlphaEarth Foundations provides a powerful new lens for understanding our planet by solving two major challenges: data overload and inconsistent information.” This sentence being the first sentence in the “How AlphaEarth Foundations Works” section of the [deepmind post]((https://deepmind.google/discover/blog/alphaearth-foundations-helps-map-our-planet-in-unprecedented-detail/)) revealing the aforementioned product to the world. I think the most important word in that sentence is **“lens”** because that is exactly what this product appears to be. 

Before we look at the embeddings lets look at the literal spatial foundation used to build them. Here is a yearly Red, Green, and Blue composite from Sentinel-2 L1C which matches the resolution (10m) of the AEF embeddings.   
<image of RGB image of Michigan, sentinel next to embeddings> 

This image is what most people imagine when they take a look at satellite imagery, its not too different from what you would see out of a plane window (albeit you may question why your pilot is flying a little too high...). Now, when you first looked at that image I bet you immediately saw features relevant to what your domain of expertise is or if you are familiar with the area you looked at regions you know personally. All of this to say this image, because of what _you know_ is worth more than just the RGB components it is made of.   

This is where we can start to look at the AEF satellite embeddings, which were produced using a model that saught to replicate that understanding by digesting an indiviudally incomprehensible level of information and distilling that into vectors that capture miniscule amounts of human comprehension.  By looking at these different embeddings as we would a Red, Green, Blue (RGB) composite image what we see are the definition of fascinating, largely because we see emergence of phenomenon we know and recognize from our own understanding.  

However, with 64 unique embedding layers, looking at every possible RGB combination (n=41,664) would take some time! 
<Gif of Michigan/GLB>
Now on the Earth Engine Developers page there are some fantastic [guides on how to use these embeddings classic LULC and remote sensing type tasks](https://developers.google.com/earth-engine/tutorials/community/satellite-embedding-01-introduction). One clear usefulness I see in this is in the similarity search space or using the embeddings visually, exactly as many have used Google Earth and Google Earth Engine for years with high resolution satellite data or products like NAIP, to enhance their geospatial dataset curation/generation/selection to train and validate models with traditional methodology and traditional inputs (e.g. data from Earth Observation Platforms like Landsat and Sentinel). What does concern me though, is the potential for many to just blindly switch over to using these embeddings as if they were their own true bands in an EO platform. The instrumentation on EO platforms are selected based on their theoretical or known relationship to phenomena in the world. The satellite embeddings, while an unprecedented representation of the Earth in a year at a 10m resolution and a consolidation of the electromagnetic spectrum in many ways, are still fundamentally a black box product. While many relationships between phenomena like biomass, crop yield, and many other important characteristics of the landscape will inevitably be made using these embeddings it’s important to consider how we can actually ground those in the scientific laws and understanding that drove the inputs that trained the model in the first place. I hope that this foundation model and others are seen as a reason why we need to maintain programs like Landsat and even produce more EO, more ground validation, and more science in general as the more **lenses** we have to view the world the more complete our understanding of its overall health and ongoing evolution can be.     
