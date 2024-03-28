# HoVer-Net(NeuLy)

This repository is dedicated to the research paper [Enhancing AI in identifying immune cell subtypes in inflammatory bowel disease H&E slides through immunohistochemistry annotations](link).

StarDist folder contains the StarDist* model described in our paper.

##HoVer-Net(NeuLy)
HoVer-Net(NeuLy) model can be downloaded [here](https://drive.google.com/file/d/19HNdi5H4V8Pr-zvX9YGWmjjDF_xI_d7E/view?usp=sharing).

type_info.json file is used for visualization of segmentation and classifiction of HoVer-Net(NeuLy).

##Usage
###Tiles
```python
python run_infer.py --nr_types=4 --type_info_path="path/to/type_info.json" --model_path="path/to/HoVer-Net(NeuLy).tar" --model_mode="fast" tile --input_dir="path/to/your/input/images" --output_dir="path/to/your/output/directory"
```
###WSI
```python
python run_infer.py --nr_types=4 --type_info_path="path/to/type_info.json" --model_path="path/to/HoVer-Net(NeuLy).tar" --model_mode="fast" wsi --input_dir="path/to/your/input/images" --output_dir="path/to/your/output/directory"
```
##Installation & prerequisities
Follow instruction from original [HoVer-Net repository](https://github.com/vqdang/hover_net) 
