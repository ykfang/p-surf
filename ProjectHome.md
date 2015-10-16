![http://wiki.p-surf.googlecode.com/hg/top.png](http://wiki.p-surf.googlecode.com/hg/top.png)

The task of ﬁnding correspondences between two images of the same scene or object is part of many computer vision applications.
Camera calibration, 3D reconstruction, image registration, and ob ject recognition are just a few. The search for discrete image correspondences – the goal of SURF (Herbert Bay, Tinne Tuytelaars, and Luc Van Gool. Surf: Speeded-up robust features. In 9th European Conference on Computer Vision, Graz, Austria, 2006) – can be divided into _three main steps_:

  * _First_, **interest points** are selected at distinctive locations in the image, such as corners, blobs, and T-junctions. The most valuable property of an interest point detector is its repeatability, i.e. whether it reliably ﬁnds the same interest points under diﬀerent viewing conditions.

  * _Next_, the neighbourhood of every interest point is represented by a feature vector. This descriptor has to be distinctive and, at the same time, robust to noise, detection errors, and geometric and photometric deformations.

  * _Finally_, the **descriptor vectors** are matched between diﬀerent images. The matching is often based on a distance between the vectors, e.g. the Mahalanobis or Euclidean distance. The dimension of the descriptor has a direct impact on the time this takes, and a lower number of dimensions is therefore desirable. In out implementation, we use a 64-feature vector to represent the neighbourhood of every interest point.

This project provides an implementation of the method in the form of a library for the Processing programming environment. The library can be used without limitations from any Java program as well.

Our implementation was tested on  _K. Mikolajczyk_**datasets. You can find it on [his site](http://www.robots.ox.ac.uk/~vgg/research/affine/index.html) or in our
[download page](http://code.google.com/p/p-surf/downloads/list).**

### Getting Started ###

[How to start](Getting_Started.md)

### Supported platforms ###

Processing SURF works on Linux, OS X and Windows.

### Some results ###

We made some tracking experiments on a Gran Prix video. See them on [our page on Vimeo](http://www.vimeo.com/processingsurf).

### Bug report ###

If you find a bug, please search if it has been already reported in our [bug tracker](http://code.google.com/p/p-surf/issues/list), otherwise feel free to report it!.

### Credits ###

[Credits page](Credits.md)