# HoVer-Net(NeuLy)

This repository is dedicated to the research paper [Immunohistochemistry annotations enhance AI identification of lymphocytes and neutrophils in digitized H&E slides from inflammatory bowel disease](link) (**under review**).

**StarDist** folder contains the *StarDist** model described in our paper. To run the model follow instructions from [original StarDist repository](https://github.com/stardist/stardist).

## HoVer-Net(NeuLy)
**HoVer-Net(NeuLy)** model can be downloaded [here](https://drive.google.com/file/d/1EQh7pE3YpBm2CMHwGQEIdSWrkcQbIV0r/view?usp=drive_link).
Model available upon reasonable request. Contact: [natalia.zurek@cshs.org](mailto:natalia.zurek@cshs.org)


*type_info.json* file is used for visualization of segmentation and classifiction of HoVer-Net(NeuLy).

## Installation & Prerequisities
Follow instructions from original [HoVer-Net repository](https://github.com/vqdang/hover_net) 

## Usage
### Tiles
```python
python run_infer.py --nr_types=4 --type_info_path="path/to/type_info.json" --model_path="path/to/HoVer-Net(NeuLy).tar" --model_mode="fast" tile --input_dir="path/to/your/input/images" --output_dir="path/to/your/output/directory"
```
### WSI
```python
python run_infer.py --nr_types=4 --type_info_path="path/to/type_info.json" --model_path="path/to/HoVer-Net(NeuLy).tar" --model_mode="fast" wsi --input_dir="path/to/your/input/images" --output_dir="path/to/your/output/directory"
```

