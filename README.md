# EquivReg
Official repo for CoRL 2021 paper **Correspondence-Free Point Cloud Registration with SO(3)-Equivariant Implicit Shape Representations** [(link)](https://proceedings.mlr.press/v164/zhu22b.html)

## Environment
After creating a virtual environment with python 3.8, inside the virtual environment, do:
1. `python setup.py build_ext --inplace`
2. Install [torch-batch-svd](https://github.com/KinglittleQ/torch-batch-svd)

## Dataset
The preprocessed ModelNet40 dataset can be downloaded at this [Google Drive link](https://drive.google.com/file/d/1XU62rCk-S9OB_Hn7Z7I0D9aUmFuHCBpz/view?usp=share_link). It is processed by this [repo](https://github.com/davidstutz/mesh-fusion) to obtain water-tight meshes and occupancy value for points in the space, which are not available in the original ModelNet40 dataset (mentioned in the OccNet repo). Extract the files and create a symbolic link named `ModelNet40_install` under the root of this repo. 

## Training and testing
Examples are given in the files `run_train.sh` and `run_test.sh`. 

## Citation
If this work is helpful for your research, please consider citing the original authors' work: 
```
@inproceedings{zhu2022correspondence,
  title={Correspondence-free point cloud registration with SO (3)-equivariant implicit shape representations},
  author={Zhu, Minghan and Ghaffari, Maani and Peng, Huei},
  booktitle={Conference on Robot Learning},
  pages={1412--1422},
  year={2022},
  organization={PMLR}
}
```
