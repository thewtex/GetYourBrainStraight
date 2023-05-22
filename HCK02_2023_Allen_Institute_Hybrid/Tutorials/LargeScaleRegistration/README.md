Back to the [Tutorials List](../../README.md#tutorials-list)

# Large Scale Registration

## Instructors

- Matt McCormick (Kitware)

## Tutorial Description

Lightsheet microscopy methods for mouse brains result in volumes that are not
feasible to register at full resolution on a standard single computer. As we
move to register rats, non-human primates and whole human brains, a scalable
registration approach is required that is not limited by the memory capacity
of modern computational nodes and the computational capability of a single
system.

The Open Microscopy Environment (OME) next-generation file format (NGFF)
addresses scalability for large, modern bioimaging microscopy in a
cloud-optimized way and with broad-based community adoption.

The open source Insight Toolkit (ITK), a widely supported, standard library
for reproducible, computational image analysis provides a proven neuroimage
registration, underlying tools such as ANTs and elastix.

In this tutorial, we will cover principles and practices for large scale
registartion that combine the OME-Zarr NGFF, Insight Toolkit, and Dask, a
distributed computing library for Python, to register neuroimages in a way
that can limit memory consumption, distribute computation, and perform a
coarse-to-fine registration that progressively aligns structures across multiple
scales.

Duration: 0.5 hours.

## Learning Outcomes

<!-- Describe here what you would like participants to learn by the end of the tutorial. -->

1. Outcome 1. Understand the need for multiscale OME-Zarr spatial metadata and how to generate this metadata.
2. Outcome 2. Understand the need for an anti-aliased approach to multiscale image generation and how to generate  these multiscale pyramids.
3. Outcome 3. Learn how to distribute registration to limit memory consumption and improve performance.

## Approach and Materials

- [Multiscale Spatial Metadata](./Multiscale_Spatial_Metadata.ipynb)
- [Anti-aliased Multiscale Pyramids](./Anti-Aliased_Multiscale_Pyramids.ipynb)
- [Distributed Registration](./Distributed_Registration.ipynb)

## Background and References

- [OME-Zarr: a cloud-optimized bioimaging file format with international community support](https://doi.org/10.1101/2023.02.17.528834)
- [OME-NGFF: a next-generation file format for expanding bioimaging data-access strategies](https://doi.org/10.1038/s41592-021-01326-w)
- [Insight Toolkit (ITK)](https://itk.org/)
- [ITK: enabling reproducible research and open science](https://doi.org/10.3389/fninf.2014.00013)
- [elastix](https://elastix.lumc.nl/)
- [ANTs](https://github.com/ANTsX/ANTs)
