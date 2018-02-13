# Globally and Locally Consistent Image Completion

Tensorflow implementation of Globally and Locally Consistent Image Completion on [celebA](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html) dataset.  
![Alt text](images/network.JPG?raw=true "network")

## What's different from the paper  
* smaller image input size (64x64)  
* smaller patch sizes  
* less number of training iteration (500,000 iterations in the paper)

## Requirements
* Opencv 2.4
* Tensorflow 1.4

## Folder Setting
```
-data
  -img_align_celeba
    -img1.jpg
    -img2.jpg
    -...
```


## Train
```
$ python train.py 
```

To continue training  
```
$ python train.py --continue_training=True
```

## Test  
```
$ python test.py --img_path=./data/test/test_img.jpg
```

<img src="images/res.gif" width="800"/>  
Use your mouse to erase pixels in the image.  
When you're done, press ENTER.  
Result will be shown in few seconds.  


## Results  
![Alt text](images/res.png?raw=true "result")
