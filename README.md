# Deformable Handwriting Transformer 
# Pytorch / Python3.7 / CUDA 10.2

Implementation of [Handwriting Transformer](https://arxiv.org/pdf/2104.03964.pdf) using [Deformable Transformer](https://arxiv.org/pdf/2010.04159.pdf)

### Download dataset
* [IAM](https://drive.google.com/file/d/1-aMqoCeq-sEfydBJd64VeBMuGnHKtKvp/view?usp=sharing)
* [RIMES](https://drive.google.com/file/d/13Zf7tsXSILDQ2el7wBY1jelRQiK_z-Ju/view?usp=sharing)

### Requirements

* Linux, CUDA>=9.2, GCC>=5.4
  
* Python>=3.7

    We recommend you to use Anaconda to create a conda environment:
    ```bash
    conda create -n deformable_detr python=3.7 pip
    ```
    Then, activate the environment:
    ```bash
    conda activate deformable_detr
    ```
  
* PyTorch>=1.5.1, torchvision>=0.6.1 (following instructions [here](https://pytorch.org/))

    For example, if your CUDA version is 9.2, you could install pytorch and torchvision as following:
    ```bash
    conda install pytorch=1.5.1 torchvision=0.6.1 cudatoolkit=9.2 -c pytorch
    ```
  
* Other requirements
    ```bash
    pip install -r requirements.txt
    ```
    
### Compiling CUDA operators
```bash
cd ./models/ops
sh ./make.sh
# unit test (should see all checking is True)
python test.py
```
