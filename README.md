# Cell Segmentation and detection Collection
this repository is a collection of cell segmentation and detection projects I have done so far
## Projects 
so far there are two projects you can read and use so feel free to experiment them !

## WBC detection and classification
for a better classification of White blood cells, a yolo model was trained in order to detect white blood cells generally and then the white blood cell is cutted out of the given image 
and given to another model to classify the type of WBC. BCCD and PBC datasets were used in order to train models mentioned.
the first file PBC_yolo_Prep_WBC contains the code related to create a "more clean" dataset out of PBC dataset by cutting white blood cell out of images so that the model dedicated to 
classifying the white blood cells can do its job better
next file PBC_test contains the usage of a trained DenseNet121 model in order to classify white blood cells
overall architecture of a model inference would be :
Data -> bccd trained yolo11 -> cutted wbcs -> wbc class detector

A more refined and easy-to-use architecture for the project will be created soon

## Breast cancer cell segmentation
just a simple straight forward implementation of u-net architecture for the purpose of segmentation of ultrasound dataset of breast cancer cancerous cell segmentation
