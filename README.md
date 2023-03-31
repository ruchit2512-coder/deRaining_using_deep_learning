# ContourletNet: A Generalized Rain Removal Architecture Using Multi-Direction Hierarchical Representation<br> (Accepted by BMVC'21)


![image](/img_repo/example.png)


[[Paper]](https://www.bmvc2021-virtualconference.com/assets/papers/0491.pdf)
[[Supplementary Material]](https://www.bmvc2021-virtualconference.com/assets/supp/0491_supp.zip)
<!-- [[Slide Download]](https://ntucc365-my.sharepoint.com/:b:/g/personal/f05943089_ntu_edu_tw/EVUaKr-l1UNDoUeuInao0RkB6kv5MDMfUcUCNp96rRZeTA?e=5LYZSC) -->

You can also refer our previous works on other low-level vision applications!

Desnowing-[[HDCWNet]](https://github.com/weitingchen83/ICCV2021-Single-Image-Desnowing-HDCWNet) (ICCV'21) and [[JSTASR]](https://github.com/weitingchen83/JSTASR-DesnowNet-ECCV-2020)(ECCV'20)<br>
Dehazing-[[PMS-Net]](https://github.com/weitingchen83/PMS-Net)(CVPR'19) and [[PMHLD]](https://github.com/weitingchen83/Dehazing-PMHLD-Patch-Map-Based-Hybrid-Learning-DehazeNet-for-Single-Image-Haze-Removal-TIP-2020)(TIP'20)<br>
Image Relighting-[[MB-Net]](https://github.com/weitingchen83/NTIRE2021-Depth-Guided-Image-Relighting-MBNet) (NTIRE'21 1st solution) and [[S3Net]](https://github.com/dectrfov/NTIRE-2021-Depth-Guided-Image-Any-to-Any-relighting) (NTIRE'21 3 rd solution)<br>


# Network Architecture

![image](/img_repo/architecture.png)



# Experimental Results
## Qualitative Evaluation
![image](/img_repo/qualitative_heavy.png)
![image](/img_repo/qualitative_moderate.png)

# Setup and environment

To generate the recovered result you need:

1. Python 3
2. CPU or NVIDIA GPU + CUDA CuDNN
3. Pytorch 1.0+

For moderate rain (trained on Rain100H dataset)
```
$ python test_real.py --ckpt ckpt/r100h --real_dir input_img/moderate
```

For heavy rain (trained on Heavy Rain dataset)
```
$ python test_real.py --ckpt ckpt/heavyrain --real_dir input_img/heavy
```
