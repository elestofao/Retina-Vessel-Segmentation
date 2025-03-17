# Retina-Vessel-Segmentation
In this project, a segmentation method was developed to extract retinal blood vessels from fundus images using the DRIVE dataset (Digital Retinal Images for Vessel Extraction). The developed method focuses on improving segmentation accuracy without using Deep Learning techniques. The methodology proposed is based on mathematical morphology.

## Method
### Preprocessing
- Extraction of green channel
- Complement of green channel
- Contrast-limited adaptive histogram equalization (CLAHE)
- Normalization of the enchanced image via subtracting the background (morphological opening) from the CLAHE result.
- Gaussian filter

### Segmentation
- Top-hat transformation with multiple kernel sizes
- Otsu's thresholding
- Morfological closing

### Postprocessing
- Connected Component Analysis

## Results
The performance of the proposed segmentation method was evaluated using the Intersection over Union
(IoU) metric, which quantifies the overlap between the segmented blood vessels and the ground truth.
The mean IoU score obtained was 0.6102.

## Process visualization
