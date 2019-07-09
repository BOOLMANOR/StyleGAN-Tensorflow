# StyleGAN-Tensorflow
Simple Tensorflow implementation of *"A Style-Based Generator Architecture for Generative Adversarial Networks"* **(CVPR 2019 Oral)**


<div align="center">
  <img src=./assets/t1.png>
</div>

### [Paper](https://arxiv.org/abs/1812.04948) | [Official code](https://github.com/NVlabs/stylegan) | [Video](https://www.youtube.com/watch?v=kSLJriaOumA&feature=youtu.be) | [FFHQ Dataset](https://github.com/NVlabs/ffhq-dataset) 

## Source code will be soon

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
> python main.py --dataset FFHQ --img_size 1024 --progressive True --batch_size 16 --phase test
```

### Draw
#### figure02-uncurated
```
python main.py --dataset FFHQ --img_size 1024 --progressive True --phase draw --draw uncurated
```

#### figure03-style-mixing
```
python main.py --dataset FFHQ --img_size 1024 --progressive True --phase draw --draw style_mix
```

#### figure08-truncation-trick
```
python main.py --dataset FFHQ --img_size 1024 --progressive True --phase draw --draw truncation_trick
```

## Our Results
### Uncurated
<div align="center">
  <img src=./assets/uncurated.jpg width=600px height=750px>
</div>

### Style mixing
<div align="center">
  <img src=./assets/style_mix.png>
</div>

### Truncation trick
<div align="center">
  <img src=./assets/truncation_trick.png>
</div>

### Generator loss graph
<div align="center">
  <img src="./assets/g_loss.png">
</div>

### Discriminator loss graph
<div align="center">
  <img src="./assets/d_loss.png">
</div>

## Reference
[Moono's StyleGAN-esimator version](https://github.com/moono/stylegan-reproduced)

## Author
[Junho Kim](http://bit.ly/jhkim_ai)
