# HoVer-Net(NeuLy)

This repository is dedicated to the research paper [Immunohistochemistry annotations enhance AI identification of lymphocytes and neutrophils in digitized H&E slides from inflammatory bowel disease](https://pubmed.ncbi.nlm.nih.gov/39306985/).

**StarDist** folder contains the *StarDist** model described in our paper. To run the model follow instructions from [original StarDist repository](https://github.com/stardist/stardist).

## HoVer-Net(NeuLy)
**HoVer-Net(NeuLy)** model can be downloaded [here](https://drive.google.com/file/d/1EQh7pE3YpBm2CMHwGQEIdSWrkcQbIV0r/view?usp=drive_link).
Model available upon reasonable request. Contact corresponding author: [arkadiusz.gertych@cshs.edu](mailto:arkadiusz.gertych@cshs.org)


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

## Citation

If you use this project in your research, please cite the following paper:

**Immunohistochemistry annotations enhance AI identification of lymphocytes and neutrophils in digitized H&E slides from inflammatory bowel disease**  
*Natalia Zurek, Yi Zhang, Dermot P.B. McGovern, Ann E. Walts, Arkadiusz Gertych*  
**Computer Methods and Programs in Biomedicine**, 2024, Vol. 257, 108423.  
DOI: [10.1016/j.cmpb.2024.108423](https://doi.org/10.1016/j.cmpb.2024.108423)  
PMID: 39306985  

### BibTeX

```bibtex
@article{Zurek2024,
  title={Immunohistochemistry annotations enhance AI identification of lymphocytes and neutrophils in digitized H&E slides from inflammatory bowel disease},
  author={Zurek, Natalia and Zhang, Yi and McGovern, Dermot P.B. and Walts, Ann E. and Gertych, Arkadiusz},
  journal={Computer Methods and Programs in Biomedicine},
  volume={257},
  pages={108423},
  year={2024},
  month={Dec},
  doi={10.1016/j.cmpb.2024.108423},
  url={https://doi.org/10.1016/j.cmpb.2024.108423},
  pmid={39306985}
}
