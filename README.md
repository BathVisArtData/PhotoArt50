#Photo-Art-50 dataset

The Photo-Art-50 dataset is a dataset of images from photos and artwork, with ground truth bounding boxes for 50 object classes. The aim is to evaluate cross-depiction object detection performance.

The dataset was originally produced by [Qi Wu](http://www.adelaide.edu.au/directory/qi.wu01) and [Hongping Cai](http://www.bristol.ac.uk/engineering/people/372003) while working under [Peter Hall](http://www.cs.bath.ac.uk/~pmh/start/home.html) at the University of Bath.

Please also see the [People-Art dataset](https://github.com/BathVisArtData/PeopleArt).

## Description
This dataset contains 50 classes of object. There are 90 to 138 images for each class, approximately half of which are photos and the other half art. The 50 classes all appear in [Caltech-256](http://www.vision.caltech.edu/Image_Datasets/Caltech256/). Some of the photos are from [Caltech-256](http://www.vision.caltech.edu/Image_Datasets/Caltech256/); the rest are from Google searches.

The artwork images came from searching using a variety of keywords to cover a wide gamut of depiction styles, e.g. "horse cartoon", "horse drawing", "horse painting", "horse sketches", "horse kid drawing", etc. All selected images have a reasonable size of a meaningful object area and there are ground-truth bounding boxes, labelled by hand, for each object.

## Files included
* {cls_id}.{cls_name}/{cls_id}.a_{img_id}.jpg: Art images for each class
* {cls_id}.{cls_name}/{cls_id}.p_{img_id}.jpg: Photo images for each class
* gt_bb/{cls_id}.txt: Ground truth file for each class

The ground truth files contain bounding boxes for each object instance as a row in [ccv](http://libccv.org/doc/doc-dpm/) format:
image_name x0 y0 w h
NB image_name might appear more than once, which means there are multiple object instances in the image.

## Copyright
Many of the images are subject to copyright. These are provided only for "data mining for non-commercial research" or other "fair dealing" [(UK Guidance)](https://www.gov.uk/guidance/exceptions-to-copyright).

## Publications
The dataset appears in the following publications:
* [Cross-depiction problem: Recognition and synthesis of photographs and artwork](http://link.springer.com/content/pdf/10.1007/s41095-015-0017-1.pdf)
* [Beyond Photo-Domain Object Recognition: Benchmarks for the Cross-Depiction Problem](http://www.cv-foundation.org/openaccess/content_iccv_2015_workshops/w6/papers/Cai_Beyond_Photo-Domain_Object_ICCV_2015_paper.pdf)
* [Learning Graphs to Model Visual Objects Across Different Depictive Styles](http://opus.bath.ac.uk/41062/2/main.pdf)
* An earlier version appeared in [Modelling Visual Objects Invariant to Depictive Style](http://www.bmva.org/bmvc/2013/Papers/paper0023/paper0023.pdf)

If you wish to cite the dataset, please use the following [citation](citation.bib).