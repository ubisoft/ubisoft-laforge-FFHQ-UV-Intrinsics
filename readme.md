© [2023] Ubisoft Entertainment. All Rights Reserved
## FFHQ-UV-Intrinsics dataset
This GitHub repository hosts **FFHQ-Intrinsic** that contains intrinsics texture maps for 10K subjects. This dataset was obtained by applying [MoSAR](https://ubisoft-laforge.github.io/character/mosar/) on the [FFHQ-UV](https://github.com/csbhr/FFHQ-UV) dataset.
To obtain the intrinsic face attributes, we first re-targeted the texture maps from [FFHQ-UV](https://github.com/csbhr/FFHQ-UV) to our own topology and resize them to 512x512. Next, we apply MoSAR to obtain the light normalization and intrinsic texture maps estimation. We then upscale these texture maps to 1K resolution and retarget them back to their original topology.
The resulting dataset, **FFHQ-Intrinsic**, is being publicly released for the research community under Creative Commons Attribution-NonCommercial-NoDerivatives license. 

**The dataset contains diffuse, specular, ambient occlusion, translucency and normal maps for 10K subjects**.

This is the first dataset that offer rich intrinsic face attributes at high resolution and at large scale, with the aim of advancing research in this field.

<p align="center">
<img src="./Data/ffhq-intrinsics-portrait.png" style="width:60%">
</p>
## Download
Once you've downloaded and extracted the file, you'll find that it's organized with a separate folder for each subject. Inside these folders are the intrinsic attributes of each subject's face.

## Use with [FLAME](https://flame.is.tue.mpg.de/) topology
The current texture maps are registred in the Hifi3D topology (https://github.com/czh-98/REALY/tree/master/HIFI3D%2B%2B). If you want to use these texture with Flame model. Please refer to this tutorial:  https://github.com/csbhr/FFHQ-UV/blob/main/README_flame2hifi3d.md

## Use with [Basel](https://faces.dmi.unibas.ch/bfm/index.php?nav=1-1-0&id=details) topology 
We will add retargeting script of the the dataset textures to  Basel topology. 

## Cite
This dataset was built using MoSAR model. If you use this datase please cite the following work: 

```
@article{dib2023mosar,
  author    = {Dib, Abdallah and Hafemann, Luiz Gustavo and Got, Emeline and Anderson, Trevor and Fadaeinejad, Amin and Cruz, Rafale M.O and Carbonneau, Marc-André},
  title     = {MoSAR: Monocular Semi-Supervised Model For Avatar Reconstruction Using Differentiable Shading},
  journal   = {ArXiv},
  year      = {2023},
}
```

© [2023] Ubisoft Entertainment. All Rights Reserved

