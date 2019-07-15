# pT1 Gland Graph Dataset (GG-pT1)
This repo contains the intestinal gland segmentation dataset from pT1 cancer patients. 
It includes:

- **Dataset**: From each image there are 26 images of cropped glands (13 normal, 13 dysplastic). 
  - image_labels.csv: Classification label for each graph and image (normal or dysplastic)
  - There is a folder for each image. In this folder there is a folder for each crop containing:
    - Cropped out gland image (*-image.jpg)
    - Annotation mask (*-gt.png)
    - Excel file with the features (*-features.xlsx)



- **Text files**: 
  - dataset_split.csv:  (reference, validation and test set)
  - feature_overview.csv: List of all possible node features (with enumeration, mean and std)



- **Graphs**:
  - Base dataset: cell segmentation with features (just nodes)
  - Paper graphs:
    - Baseline
    - Optimized graph



This dataset is submitted for publishing at the [COMPAY19 Workshop](https://openreview.net/group?id=MICCAI.org/2019/Workshop/COMPAY).
The parameters for the GED calculated in this paper can be found [here](https://bit.ly/2xDuRcV)


If you want to cite us please use:
`` BIBTEX TBA``

