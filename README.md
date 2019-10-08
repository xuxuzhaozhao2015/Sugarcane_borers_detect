Object category detection 
===================================


Package contents
----------------

The project runs in MATLAB and uses
[MatConvNet](http://www.vlfeat.org/matconvnet) and
[VLFeat](http://www.vlfeat.org). This package contains the following
MATLAB functions:

* `boxinclusion.m`: compute the inclusion of bounding boxes.
* `boxoverlap.m`: compute the overlap of bounding boxes.
* `boxsuppress.m`: non-maxima box suppression.
* `detect.m`: sliding window detector.
* `detectAtMultipleScales.m`: an intermediate example detector.
* `evalDetections.m`: evaluate detections using the PASCAL VOC criterion.
* `evaluateModel.m`: evaluate a detector against a database of images.
* `extract.m`: extract HOG features from bounding boxes.
* `loadData.m`: load practical data.
* `setup.m`: setup MATLAB environment.

Appendix: Installing from scratch
---------------------------------

The project requires both VLFeat and MatConvNet. VLFeat comes with
pre-built binaries, but MatConvNet does not.

1. From Bash, run `./extras/download.sh`. This will download the
   German Street Sign Benchmark data and VLFeat.
2. From MATLAB, run `addpath extras ; prepareLabData.m`.

Changes
-------

* *2014a* - Initial edition

License
-------
