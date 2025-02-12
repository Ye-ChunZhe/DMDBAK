# DMDBAK
This repo is the official implementation for <mark>Benchmark for Human Back Acupuncture Point Detection:Comprehensive Algorithmic Evaluation</mark>.

# Benchmark for Human Back Acupuncture Point Detection
A publicly available dataset specialized for the detection of keypoints on human back acupoints has been pioneered and constructed by this paper: DMD-BAK(*Data science,Machine learning & Dynamical control:Back Acupoints Keypoints*).

The performance of deep learning keypoint detection networks with different paradigms, architectures, and features on the back acupoint dataset was comprehensively analyzed by this paper.

# Overall architecture for human back acupuncture point dataset construction and evaluation of various algorithms
![image](src/1_flow_chart/1_flow_chart_page-0001.jpg)

# Comparison of prediction results
![image](src/5_same_image/5_same_image_page-0001.jpg)

# Data Preparation
### Please download our public dataset first
Our dataset website is available at https://www.kaggle.com/datasets/chunzheye/dmd-bak.
### Data Processing
Process the downloaded dataset into coco or yolo format, our code handles coco format.
- Put downloaded data into the following directory structure:
```
  - backacupoint_data/
    - images/
      -all_images
    - labelme_jsons/
      -all_jsons

- Split dataset:
```
python tools/dataset/split_dataset.py
