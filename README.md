### Project Description

+ Project title: Predictive analytics, model evaluation and selection
+ This project is conducted by Jongyoon Sohn

In this project, I will carry out **model evaluation and selection** for predictive analytics on image data. As data scientists, we often need to **evaluate** different modeling/analysis strategies and decide what is the best. Such decisions need to be supported by sound evidence in the form of *model assessment, validation and comparison*. In addition, we also need to **communicate our decision and supporting evidence** clearly and convincingly in an accessible fashion.

### Datasets

[A set of 2,500 facial images with 22 different emotions](https://www.dropbox.com/s/kvi949ea1rey1d8/train_set.zip?dl=0).

### Challenge

Your client is interested in creating an mobile AI program that **accurately recognizes the emotion from facial images**.  The portability of this AI program (holding storage and memory cost) and the computational efficiency (test running time cost) are of great concern to your client. This translates to a balance between the complexity of variable/features/models used and the predictive performance.

![image](figs/predictiveprogram.png)

Assume that the **current practice** on your client side is just using [boosted](https://en.wikipedia.org/wiki/Boosting_(machine_learning)) [decision stumps](https://en.wikipedia.org/wiki/Decision_stump) on facial landmark features (see Tutorial for more detail). `R` pakcage [`gbm`](https://cran.r-project.org/package=gbm) can be used to implement this classifier.

+ Project summary: In this project, I created a classification engine for facial emotion recognition. For the baseline model, I used a gbm model for which we learned the best hyperparameters. For the improved model, XGBoost was applied with some improvement but for the final model I tried to manipulate a Neural Network algorithm that learned from the pairwise distances of fiducial points in each image.

Following [suggestions](http://nicercode.github.io/blog/2013-04-05-projects/) by [RICH FITZJOHN](http://nicercode.github.io/about/#Team) (@richfitz). This folder is orgarnized as follows.

```
proj/
├── lib/
├── data/
├── doc/
├── figs/
└── output/
```

Please see each subfolder for a README file.
