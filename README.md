# Entity Neural Network Zoo

[![Actions Status](https://github.com/entity-neural-network/enn-zoo/workflows/Checks/badge.svg)](https://github.com/entity-neural-network/enn-zoo/actions)
[![Discord](https://img.shields.io/discord/913497968701747270?style=flat-square)](https://discord.gg/SjVqhSW4Qf)


The enn-zoo package collects [entity-gym](https://github.com/entity-neural-network/entity-gym) bindings for a number of reinforcement learning environments:
- [Procgen](https://github.com/openai/procgen)
- [Griddly](https://github.com/Bam4d/Griddly)
- [MicroRTS](https://github.com/santiontanon/microrts)
- [ViZDoom](https://github.com/mwydmuch/ViZDoom)
- [CodeCraft](https://github.com/cswinter/DeepCodeCraft)

## Setup

```
git clone https://github.com/entity-neural-network/enn-zoo.git
cd enn-zoo
poetry install
poetry run pip install setuptools==59.5.0
poetry run pip install torch==1.10.2+cu113 -f https://download.pytorch.org/whl/cu113/torch_stable.html
poetry run pip install torch-scatter -f https://data.pyg.org/whl/torch-1.10.0+cu113.html
```

Some of the environments have additional dependencies:

```
sudo apt install python3-dev make build-essential libssl-dev zlib1g-dev \
libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm \
libncursesw5-dev xz-utils tk-dev libxml2-dev libxmlsec1-dev libffi-dev liblzma-dev
```

## Usage

```
poetry run enn_zoo/train.py
```
