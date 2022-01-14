# hack2022-12-cosmetic
# Challenge 12: Automated Artefact Removal in Multiplexed Fluorescence Images for Cosmetic Purposes

### *Create a model that visually suppresses debris in multiplexed fluorescence images for improved representation*

## Challenge Description: 
Image and sample artefacts are common in microscopy images. Although automatic detection helps to filter out the affected cells for quantification, visual appearance is still hampered and is most evident in viewing multiple channels in 3D. Artefacts will also hamper in qualitative analysis and are distracting when presented in front of an interdisciplinary audience who may not be used to interpreting them. This challenge aims to develop tools to automatically remove artefacts such as lint and fluorescent antibody blobs in a similar way that the Photoshop clone tool reduces cosmetic aberrations in photographs. NOTE: The resulting images are not expected to be used for quantitative analysis.

## Background:
It is common to observe anomalies in microscopy images, here termed as image artefacts. They may emit fluorescence or alter the optical path of the microscope such that the underlying signal from the sample is corrupted and modified. As such, identifying cell states and populations is hindered as these rely on accurate quantification of fluorescence signals with high signal-to-background ratios. Even where image quantification is not the main goal, exploratory exercises are hampered when there are abundant artefacts that distract end users. This is especially true for users who may be unfamiliar with recognizing artefacts in biomedical images, which may lead to misinterpretation. The artefacts found in this challenge can be classified into 3 categories: <br>

* Lint - these look like filamentous fibers of varying length that are believed to originate from the handling of the samples or dust particles in the air.<br>
* Blobs - these are round, small and bright aggregates of fluorescent antibodies that have the tendency to overinflate the mean intensity signal from any underlying cells making them appear to highly express the protein of interest.<br>
* Tile artefacts - these have dim aura-like patterns that also inflate the mean intensity signal of cells but over a larger area (see blobs). These are caused by fluorescent objects that are out-of-focus. Because they are defocused, they may only affect one imaging tile or field of view. Therefore, they have sharp edges at the borders of the image tiles.<br>


## Ground truth annotations and data provided: 
Manual annotations of artefacts (lint, fluorescent blobs, illumination tiles) and corresponding fluorescence images of various registered markers in colorectal tissue

## Compute requirements:
GPU: ie 1080GTX, 3070 RTX, etc 
RAM: 64GB

## Recommended software:
Fiji or Napari
If programming in Python, install scikit-image, opencv, Tensorflow, PyTorch
If programming in MATLAB, install image processing toolbox
