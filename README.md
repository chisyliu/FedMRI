# FedMRI

# [Specificity-Preserving Federated Learning for MR Image Reconstruction]( )

> **Authors:** 
> [Chun-Mei Feng](https://scholar.google.com.hk/citations?user=g2nqHBcAAAAJ&hl=zh-CN), 
> [Yunlu Yan](), 
> [Huazhu Fu](http://hzfu.github.io/), 
> [Yong Xu](https://scholar.google.com.hk/citations?user=zOVgYQYAAAAJ&hl=zh-CN), and 
> [Ling Shao](http://www.inceptioniai.org/).


[[Paper]( )][[Code](https://github.com/chunmeifeng/FedMRI)]

## Dependencies
* numpy==1.18.5
* scikit_image==0.16.2
* torchvision==0.8.1
* torch==1.7.0
* runstats==1.8.0
* pytorch_lightning==1.0.6
* h5py==2.10.0
* PyYAML==5.4

## Data Prepare

Download data from the link https://fastmri.org/dataset/, https://www.med.upenn.edu/sbia/brats2018/data.html 

[[Training code --> FedMRI](https://github.com/chunmeifeng/FedMRI)]

`git clone https://github.com/chunmeifeng/FedMRI.git`

## Train
single gpu train:
"python ixi_train_t2net.py"

multi gpu train :
you can change the 65th line in ixi_tain_t2net.py , set num_gpus = gpu number, then run
"python ixi_train_t2net.py"


**single gpu train**
```bash
python ixi_train_t2net.py
```

**multi gpu train**
you can change the 65th line in ixi_tain_t2net.py , set num_gpus = gpu number, then run
```bash
python ixi_train_t2net.py
```

###  :fire: NEWS :fire:
* We have upload the mask file. 
* Before our project, you need to  transform the .nii file to .mat file at first.  
* We have provided the code of converting the .nii file to .mat file.


## Citation

```
@inproceedings{feng2021,
  title={Specificity-Preserving Federated Learning for MR Image Reconstruction},
  author={Feng, Chun-Mei and Yan, Yunlu and Fu, Huazhu and Xu, Yong and Ling, Shao },
  journal={arXiv e-prints},
  pages={arXiv--2106},
  year={2021}
}
```


