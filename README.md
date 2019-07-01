# StyleGAN-Tensorflow
Simple Tensorflow implementation of *"A Style-Based Generator Architecture for Generative Adversarial Networks"* **(CVPR 2019 Oral)**

### [Paper](https://arxiv.org/abs/1812.04948) | [Official code](https://github.com/NVlabs/stylegan) | [Video](https://www.youtube.com/watch?v=kSLJriaOumA&feature=youtu.be) | [FFHQ Dataset](https://github.com/NVlabs/ffhq-dataset) 

## Will be soon

## Usage
```
├── dataset
   └── YOUR_DATASET_NAME
       ├── 000001.jpg 
       ├── 000002.png
       └── ...
```

### Train
```
> python main.py --dataset FFHQ --img_size 1024 --gpu_num 4 --progressive True --phase train
```

### Test
```
> python main.py --dataset FFHQ --img_size 1024 --progressive True --phase test
```

## Reference
[Moono's StyleGAN-esimator version](https://github.com/moono/stylegan-reproduced)

## Author
[Junho Kim](http://bit.ly/jhkim_ai)
