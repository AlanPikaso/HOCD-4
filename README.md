# HOCD-4: Handheld Orchard Citrus Disease Dataset

HOCD-4 (Handheld Orchard Citrus Disease Dataset) is a self-collected citrus disease detection dataset designed for object detection tasks under real close-range orchard imaging conditions. The dataset contains citrus leaf and fruit disease images captured using a handheld smartphone in real orchards.

The dataset was constructed to support research on lightweight and robust citrus disease detection models, especially for practical orchard inspection scenarios involving small disease regions, background clutter, occlusion, overlapping leaves or fruits, and natural illumination variation.

## Dataset Overview

HOCD-4 contains **3,511 high-resolution images** with an original resolution of **1920 × 1080**. The images were collected from **12 orchard bases** located in the main production area of Bingtang sweet orange in Yongxing County, Chenzhou City, Hunan Province, China.

All images were manually captured at close range using a **HUAWEI P40 5G smartphone** under natural illumination conditions without using a flash. Image acquisition was conducted between **1 January 2023 and 26 March 2024**.

The dataset includes visible disease symptoms on both citrus leaves and fruits.

## Disease Categories

HOCD-4 covers four typical citrus disease categories:

| Class ID | Disease Category | Description |
|---|---|---|
| 0 | HLB | Huanglongbing / citrus greening |
| 1 | Melanose | Citrus melanose |
| 2 | Canker | Citrus canker |
| 3 | Black Spot | Citrus black spot |

The disease categories were confirmed with the assistance of agricultural experts based on visible field symptoms.

## Dataset Statistics

The dataset was divided into training, validation, and test sets at a ratio of 8:1:1.

| Category | Training Set | Validation Set | Test Set | Total | Proportion (%) |
|---|---:|---:|---:|---:|---:|
| HLB | 906 | 113 | 113 | 1,132 | 32.24 |
| Melanose | 670 | 84 | 83 | 837 | 23.84 |
| Canker | 640 | 80 | 80 | 800 | 22.79 |
| Black Spot | 594 | 74 | 74 | 742 | 21.13 |
| **Total** | **2,810** | **351** | **350** | **3,511** | **100.00** |

## Annotation Format

The dataset is annotated in the YOLO object detection format.

Each image has a corresponding `.txt` annotation file with the same base filename. Each line in an annotation file follows the format:

```txt
<class_id> <x_center> <y_center> <width> <height>
