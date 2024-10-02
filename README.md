# AI Group Research Project: Brain Tumor Segmentation

**Class Name:** Your Class Name Here

## Problem Statement
The objective of this project is to develop a robust classification system for brain tumor detection using medical imaging datasets. The challenge is to classify images into binary tumor present vs. tumor absent while providing feedback on the tumor’s location in the image. The project will be divided into three roles, with each team member focusing on different methodologies to enhance classification accuracy and interpretability.

## Methodologies
The project will focus on image segmentation, utilizing the Pytorch and MONAI frameworks. The main goal is to accurately identify and locate tumor regions within the brain scans, providing a clear visual for any potential clinical decision-making applications. The current neural architecture focus will revolve around U-Net implementation; however, if time allows, the group plans on comparing and contrasting different architecture types.

## Experimental Setup
The dataset will be gathered from the website: [medicaldecathlon.com](http://medicaldecathlon.com), titled “Gliomas segmentation necrotic/active tumor and oedema.” The following are attributes of the dataset alongside some basic definitions to better describe it.

### Attributes
- **Target:** Gliomas segmentation necrotic/active tumor and oedema
- **Modality:** Multimodal multisite MRI data (FLAIR, T1w, T1gd, T2w)
- **Size:** 750 4D volumes (484 Training + 266 Testing)
- **Source:** BRATS 2016 and 2017 datasets
- **Challenge:** Complex and heterogeneously-located targets

### Vocabulary
- **Gliomas:** A group of tumors that arise from glial cells in the Central Nervous System.
- **Glial:** A cell of the nervous system that serves a homeostatic (maintain environment) role (supporting cells).
- **Oedema:** Swelling, accumulation of fluid. Tumor causes the swelling.

Currently, the group anticipates spending the majority of the time preparing the data to pass through the mentioned frameworks. The original dataset comes packaged in "NIFTI" files, an open file format commonly used to store brain imaging data obtained using MRI methods. Fortunately, there exists some open-source code that can convert 3D MRI "NIFTI" file types into a readable format such as "DICOM" images. Unfortunately, our dataset comes in a 4D MRI format that represents the standard: Width, Height, and Depth dimensions, but provides an extra dimension of time typically used to track blood flow. Some extensive research will be done to see if the added dimension would help us in achieving our goal or if it would only add unnecessary complexity.

Lastly, once the DICOM image types are processed, we plan on utilizing the OpenCV framework to further process the data by removing unnecessary pixels by applying some edge detection filtering techniques.

## References
1. [Article 1](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7778711/pdf/12065_2020_Article_540.pdf)
2. [Article 2](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6945006/pdf/ns-1938396-198.pdf)
3. [Article 3](https://www.sciencedirect.com/science/article/pii/S2352914821002033?via%3Dihub)
4. [Article 4](https://journalofbigdata.springeropen.com/articles/10.1186/s40537-021-00444-8)
5. [Article 5](https://arxiv.org/pdf/1906.01796v2)
