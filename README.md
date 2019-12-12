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
  - dataset_split.csv: reference, validation and test set split for all 4 cross-validations
  - feature_overview.csv: list of all possible node features (with enumeration, mean and std)
  - ged-costs.csv: parameters for the different experiments



- **Graphs**:
  - Base dataset: cell segmentation with features (just nodes)
  - Paper graphs:
    - Baseline
    - Optimized graph



This dataset has been for published at the [COMPAY19 Workshop](https://openreview.net/group?id=MICCAI.org/2019/Workshop/COMPAY) ([link to the paper](https://openreview.net/pdf?id=HklExX79-S)).
The parameters for the GED calculated in this paper can be found [here](https://bit.ly/2xDuRcV).

The current state-of-the-art performance is 83.3±1.7 on the 4-fold CV. If you outperform this, let me know and I will add you to the list.

| Published by  | Paper       | Used method | Performance |
|---------------|-------------|-------------|-------------|
| Studer et al. | ([COMPAY Workshop @ MICCAI 2019](https://openreview.net/pdf?id=HklExX79-S)). | Improved bipartite graph-matching | 83.3±1.7 |

If you use this dataset in your publication cite this paper:

``@inproceedings{studer2019graph,
  title={Graph-based Classification of Intestinal Glands in Colorectal Cancer Tissue Images},
  author={Studer, Linda and Toneyan, Shushan and Zlobec, Inti and Dawson, Heather and Fischer, Andreas},
  year={2019}
  booktitle={COMPAY Workshop, International Conference on Medical Image Computing and Computer-Assisted Intervention},
  year={2019},
}``

This work is part of a larger project. Find out more [here](https://icosys.ch/bts-project).

