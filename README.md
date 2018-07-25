# Glow
Pytorch implementation of OpenAI's generative model [GLOW](https://github.com/openai/glow). This repo provides a modular / clean approach for stacking invertible transformations. 

## Running Code
```
python train.py <args>
```
e.g.
```
CUDA_VISIBLE_DEVICES=0 python train.py --depth 10 --coupling affine --batch_size 64 --print_every 100 --permutation conv
```
## TODOs
- [ ] Multi-GPU support. If performance is an issue for you, I encourage you to checkout [this](https://github.com/chaiyujin/glow-pytorch) pytorch implementation. It seems to offer more features, at the expense of being slighlty more cumbersome. 
- [ ] Support for more datasets
- [ ] LU-decomposed invertible convolution. 
