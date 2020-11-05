# GaitGANv2
GaitGANv2 is a new method based on generative adversarial network to remove variations for gait recognition.  Our approach differs from the traditional GAN in that GaitGANv2 contains two discriminators instead of one. They are respectively called fake/real discriminator and identification discriminator. While the first discriminator ensures that the generated gait images are realistic, the second one maintains the human identity information.
Link to paper:
- [GaitGANv2: Invariant Gait Feature Extraction Using Generative Adversarial Networks](http://r.web.umkc.edu/rlyfv/papers/gaitganv2.pdf)
Please contact with me (rijun.liao@gmail.com) if you have any questions. Thank you!

## Prerequisites

- Caffe
- Python
- GPU

## Dataset & Preparation
- Step 1: Download [CASIA-B GEI Dataset](http://www.cbsr.ia.ac.cn/english/Gait%20Databases.asp)
- Step 2: Prepare training dataset, the left image is the source image while the right image is the target image, here the samples on folder of "sampes_of_training_data"

## Train
```bash
sh run_lstm_RGB.sh
```

## Citation
Please cite these papers in your publications if it helps your research:
```
@Article{yu2019gaitganv2,
  Title                    = {{GaitGANv2}: Invariant Gait Feature Extraction Using Generative Adversarial Networks},
  Author                   = {Yu, Shiqi and Liao, Rijun and An, Weizhi and Chen, Haifeng and Reyes, Edel B Garc{\'\i}a and Huang, Yongzhen and Poh, Norman},
  Journal                  = {Pattern recognition},
  Year                     = {2019},
  Pages                    = {179--189},
  Volume                   = {87},
  Publisher                = {Elsevier}
}
```

## Acknowledgments
This code was based on the source of [LRCN_activity_recognition](https://github.com/intel/caffe/tree/master/examples/LRCN_activity_recognition)
