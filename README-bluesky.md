# 补充说明

## 首次安装和运行

- `python -m venv venv`, 创建venv到./venv目录，仅第一次需要
- `.\venv\Scripts\Activate.ps1`，使用venv
- 根据README进行安装
  - README里的"[pytorch](https://pytorch.org) <3"等里头的"<3"，是爱心的意思，不是版本号的意思
  - 其中torch要装CUDA build（支持GPU），pip install装的版本默认是不支持GPU的，选带"CUDA"标识的：https://pytorch.org/get-started/locally/
- 根据README运行
  - `python train.py config/train_shakespeare_char.py --compile=False`，要加"--compile=False", Windows下不支持compile优化

## 后续运行

- `.\venv\Scripts\Activate.ps1`，使用venv
- `python train.py config/train_shakespeare_char.py --compile=False`，要加"--compile=False", Windows下不支持compile优化