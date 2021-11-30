# Deformable Handwriting Transformer (Pytorch / Python3)

Implementation of [Handwriting Transformer](https://arxiv.org/pdf/2104.03964.pdf) using [Deformable Transformer](https://arxiv.org/pdf/2010.04159.pdf)

### Download dataset
* [IAM](https://drive.google.com/file/d/1-aMqoCeq-sEfydBJd64VeBMuGnHKtKvp/view?usp=sharing)
* [RIMES](https://drive.google.com/file/d/13Zf7tsXSILDQ2el7wBY1jelRQiK_z-Ju/view?usp=sharing)

### Compiling CUDA operators
```bash
cd ./models/ops
sh ./make.sh
# unit test (should see all checking is True)
python test.py
```
