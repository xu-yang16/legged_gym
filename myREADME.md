## Getting Started
```bash
conda create -n legged python=3.8
conda activate legged
which pip
pip install torch==1.10.0+cu113 torchvision==0.11.1+cu113 torchaudio==0.10.0+cu113 -f https://download.pytorch.org/whl/cu113/torch_stable.html
wget https://cloud.tsinghua.edu.cn/f/36660a82fd344874be10/?dl=1
tar -zxvf IsaacGym_Preview_4_Package.tar.gz .
cd IsaacGym_Preview_4_Package/isaacgym/python 
pip install -e .
cd examples && python 1080_balls_of_solitude.py

# install rsl_rl
git clone https://github.com/leggedrobotics/rsl_rl.git
cd rsl_rl && pip install -e .

# install legged_gym
git clone https://github.com/xu-yang16/legged_gym.git
cd legged_gym && pip install -e .
```

## How to use
```bash
conda activate legged
python scripts/train.py --task=anymal_c_flat
python scripts/play.py --task=anymal_c_falt

python scripts/train.py --task=cassie
python scripts/play.py --task=cassie
```
