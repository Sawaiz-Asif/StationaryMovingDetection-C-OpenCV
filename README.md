Object Detection and Classification in Video Sequences

Introduction

This project enhances the understanding and capabilities in object detection and classification within video sequence analysis. Building on previous work in foreground-background segmentation, this assignment introduces refined methods for blob extraction, statistical classification, and stationary foreground extraction, with a focus on practical applications over theoretical analysis.
Methods
A. Blob Extraction

    Sequential Grass-Fire Algorithm: Utilized for its effectiveness in identifying and isolating connected components in binary images.

B. Blob Filtering

    Size Thresholds: Filters out insignificant objects, retaining only those with notable dimensions for further analysis.

C. Blob Classification

    Statistical Models: Applies models to categorize detected blobs into specific groups like people, cars, etc., based on their aspect ratios using Weighted Euclidean Distance (WED).

D. Extracting Stationary Foreground Objects

    Duration and Movement Analysis: Differentiates static from moving objects by analyzing pixel presence in the foreground over time.

Implementation

Each method is implemented with specific functions designed to optimize the object detection and classification process:

    extractBlobs: Blob extraction from binary images.
    removeSmallBlobs: Filtering out blobs that don't meet specified size criteria.
    classifyBlobs: Categorizing blobs into predefined groups based on aspect ratios.
    extractStationaryFG: Identifying stationary objects in video footage.

Data

The methodologies were tested using four key datasets to ensure robustness across diverse scenarios:

    AVSS2007
    ETRI Dataset
    PETS2006
    VISOR

Results and Analysis

The system was evaluated on its ability to detect stationary objects with different threshold values, demonstrating the importance of fine-tuning parameters to balance detection accuracy and computational efficiency.
Conclusions

The project confirmed the effectiveness of the developed methodologies in improving object detection and classification within video sequences. Future work could focus on refining these techniques and exploring advanced methods like deep learning for enhanced performance.


References

D. Ortego and J. C. SanMiguel, ”Stationary foreground detec-
tion for video-surveillance based on foreground and motion his-
tory images,” 2013 10th IEEE International Conference on Ad-
vanced Video and Signal Based Surveillance, Krakow, Poland,
2013, pp. 75-80, doi: 10.1109/AVSS.2013.6636619
