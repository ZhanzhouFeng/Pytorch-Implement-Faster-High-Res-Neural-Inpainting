# Pytorch-Implement-Faster-High-Res-Neural-Inpainting
 This is a Pytorch implementation for paper "High-Resolution Image Inpainting using Multi-Scale Neural Patch Synthesis"
 
### Version

* `python`   		3.6/3.7

* `pytorch`		 1.1.0
* `torchvision`        0.3.0  
* `opencv-python`    4.2.0.32

### Examples


![teaser](/overall_result/results/result1.jpg "Sample inpainting results on Paris StreetVeiw images")

![teaser](/overall_result/results/5.jpg "Sample inpainting results on Paris StreetVeiw images")

This is the python code for [High-Resolution Image Inpainting using Multi-Scale Neural Patch Synthesis](https://arxiv.org/pdf/1611.09969). The code is adapted from  [Faster-High-Res-Neural-Inpainting](https://github.com/leehomyc/Faster-High-Res-Neural-Inpainting/). Given an image, we use the content and texture network to jointly infer the missing region.

### Demo

- Download the [pre-trained models](https://drive.google.com/open?id=0BxYj-YwDqh45XzZVTXF1dnJXY28) for the content and texture networks and put them under the folder model/.

- Run the Demo
```Shell
  cd Pytorch-Implement-Faster-High-Res-Neural-Inpainting
  # This will use the trained model to generate the output
  python run_your_pic.py --content_path "Path of your picture"
  # Because sample models we provided was trained on 6000 pictures from dataset Paris StreetView,
  # We recommend that you use pictures with street views to run the demo.
  # For your convenience, we provide Street pictures not in the 
  # training set for you to run the demo in the folder "For_test"
```
- The results will be in the result fold which including some intermediate results. The final reulst will be named as "result". 

### Reference

[1]. `Yang, Chao and Lu, Xin and Lin, Zhe and Shechtman, Eli and Wang, Oliver and Li, Hao. High-Resolution Image Inpainting using Multi-ScaleNeural PatchSynthesis[C].//The IEEE Conference on Computer Vision and Pattern Recognition (CVPR) 2017`
