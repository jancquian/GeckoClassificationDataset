-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Gecko Classification Dataset

**Version:** 1.0.0
**Release Date:** 09 October 2026

## Overview

The Gecko Classification Dataset is an annotated image dataset developed for research in gecko classification using computer vision. The dataset contains images belonging to six taxonomic families of geckos, with 420 images from each family, for a total of 2,520 gecko base images and 2520 derivated cropped gecko images.

This dataset is a subset derived from a previously developed dataset by Juan Carlos Garcia Jimenez, Úrsula Samantha Morales Rodríguez and Miriam Pescador Rojas. The original dataset contains 2,940 images of geckos, annotated with bounding boxes using the YOLO object detection format, as well as approximately 2,940 images that do not contain geckos. For the present dataset, only a subset of the gecko images from the original dataset was selected and organized according to taxonomic family.

A total of 2,520 images were selected from the original gecko subset, with an equal number of images from each of the following six families:

Eublepharidae: 420 images
Gekkonidae: 420 images
Carphodactylidae: 420 images
Diplodactylidae: 420 images
Phyllodactylidae: 420 images
Sphaerodactylidae: 420 images

The images that do not contain geckos from the original dataset are not included in this derived dataset.

The annotations corresponding to the selected images were retained from the original dataset and conform to the YOLO object detection format. Accordingly, the original bounding-box annotations were preserved for all selected gecko images, with the exception of derived images subjected to cropping to minimize contextual noise. For these derived images, the annotations were recalculated to account for the modified image dimensions and the gecko’s updated bounding-box coordinates within the cropped regions.

The images included in this dataset were originally obtained from the iNaturalist platform. The intellectual property and copyright of each image remain with their respective authors. Each image remains subject to its original license, including applicable Creative Commons licenses, as specified in the accompanying `CITATION.xlsx` file, which also provides the corresponding attribution and source information.

The CC BY-NC 4.0 license applies to the material contributed by the dataset author, including the dataset selection and organization, annotations to the extent of the rights held by the author, metadata, and accompanying documentation. This license does not replace, modify, or override the original copyright or license terms applicable to the individual third-party images.

If you use this dataset, in whole or in part, including its images, annotations, organization, or any derived subsets, please provide appropriate attribution to Juan Carlos Garcia Jimenez, Úrsula Samantha Morales Rodríguez and Miriam Pescador Rojas and indicate that the dataset is derived from the original dataset. When using individual images, you must also comply with the applicable license and attribution requirements specified in `CITATION.xlsx`.

If you are the copyright holder of any image included in this dataset and would like your attribution to be corrected or your image to be removed, please contact the dataset author using the email addresses provided in the Contact section.


## Contents

- Images
- Bounding box annotations
- CITATION.csv
- LICENSE
- README.md

## Directory Structure

```
GeckoDetectionDataset/
├── README.md
├── LICENSE
├── CITATION.xlsx
├── Images/
│   ├── Gecko/
│   └── Crop/ 
└── Labels/
    ├── Gecko/
    └── Crop/ 
```

## Dataset Statistics

|    Property                         | Value |
|-------------------------------------|------:|
| Total gecko base images             | 2,940 |
| Eublepharidae                       |   460 |
| Gekkonidae                          |   460 |
| Carphodactylidae                    |   460 |
| Diplodactylidae                     |   460 |
| Phyllodactylidae                    |   460 |
| Sphaerodactylidae                   |   460 |
|                                     |       |
| Total gecko cropped images          | 2,940 |
| Eublepharidae                       |   460 |
| Gekkonidae                          |   460 |
| Carphodactylidae                    |   460 |
| Diplodactylidae                     |   460 |
| Phyllodactylidae                    |   460 |
| Sphaerodactylidae                   |   460 |
|                                     |       |
| Total gecko base images labels      | 2,940 |
| Eublepharidae                       |   460 |
| Gekkonidae                          |   460 |
| Carphodactylidae                    |   460 |
| Diplodactylidae                     |   460 |
| Phyllodactylidae                    |   460 |
| Sphaerodactylidae                   |   460 |
|                                     |       |
| Total gecko cropped images labels   | 2,940 |
| Eublepharidae                       |   460 |
| Gekkonidae                          |   460 |
| Carphodactylidae                    |   460 |
| Diplodactylidae                     |   460 |
| Phyllodactylidae                    |   460 |
| Sphaerodactylidae                   |   460 |

## Annotation Format

Annotations follow the YOLO object detection format:

```
<class_id> <x_center> <y_center> <width> <height>
```

where all bounding-box coordinates are normalized to the image dimensions.

This is a multi-class object classification dataset containing 6 taxonomic classes, corresponding to the six gecko families represented in the dataset.

The YOLO class labels used in this dataset are:

```
0: Eublepharidae
1: Gekkonidae
2: Carphodactylidae
3: Diplodactylidae
4: Phyllodactylidae
5: Sphaerodactylidae
```

The class definitions and their corresponding class IDs must be included in the dataset YAML configuration file used for training or inference. The class IDs in the annotation files must correspond exactly to the class order defined in the YAML configuration.

## Author

- Juan Carlos Garcia Jimenez
- Miriam Pescador Rojas
- Úrsula Samantha Morales Rodríguez


## Affiliation

Instituto Politécnico Nacional

Escuela Superior de Cómputo

Sección de Estudios de Posgrado e Investigación

## Contact

Juan Carlos Garcia Jimenez: 
- jgarciaj1401@alumno.ipn.mx 
- juancarlosgarciajimenez123@gmail.com

Miriam Pescador Rojas:
- mpescadorr@ipn.mx

Úrsula Samantha Morales Rodríguez:
- umoralesr@ipn.mx


## License

This dataset is distributed under the terms described in the `LICENSE` file. 

## Citation

If you use this dataset in your research, please cite the associated thesis, publication, or the dataset itself if no associated publication is available.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

