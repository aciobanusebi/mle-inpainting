# Abstract

Current approaches involve deep learning in solving this task. We propose a meta-algorithm in which we can set a probabilistic distribution on images. The set distribution can be a classic one, e.g. Normal distribution, or a modern one, e.g. PixelCNN++. Our first observation is relatively unexpected: if a learnt distribution generates reasonable images, then this does not make it is a good candidate for inpainting via our proposed algorithm and vice-versa (if a learnt distribution gives reasonable results on image inpainting via our algorithm, then this does not make it is a good candidate for sampling a new image). Our second observation is that although the visual results of the state-of-the-art method are superior than ours, the training time for our method is lower. Hence, one can experiment faster with our method to see, for example, if the desired inpainting is learnable. Moreover, using a specific distribution, our algorithm can be trained also on high quality RGB images, like 1024 times 1024 pixels. As for the experiments, we included visual results.

# Index words

Image inpainting , Probabilistic Machine Learning, Normal Distribution, Matrix Normal Distribution, PixelCNN

# Code and demo

for mle-inpainting-small-medium.ipynb

**1. Find and select the cell called "END OF CODE: RUN UP TO NOW (Ctrl + F8)".
2. Run the code below this cell (e.g, press Ctrl + F8).**
3. If you want to train a model and save a model to your Google Drive account, go to "Save models" and follow the instructions from there.
4. If you want to train a model and let it in memory, go to "Train a model" and follow the instructions from there.
5. If you want to sample images from a trained model (from your Google Drive, from my trained models or from memory), go to "Sample" and follow the instructions from there.
**6. If you want to inpaint an image, go to "Test" and follow the instructions from there.**

for mle-inpainting-large.ipynb
1. If you want to train a model and save a model to your Google Drive account, go to "Train" and follow the instructions from there.
**2. If you want to inpaint an image, go to "Test" and follow the instructions from there.**

Observation: Be sure that there is a "bugSwap" global variable (optionally set to True) if you use one of my models and that there is no "bugSwap" variable if you train your own. This affects the "Matrix Normal Channels (Faster), k=1" model's results.

Link to my trained models + 10 test images for CelebA-HQ (the archive is downloaded implicitly when needed if you use the notebook): https://drive.google.com/file/d/1Rr0AMwE9jN57EPc8LABRDqaSwDdMjy3d/view?usp=sharing

Link only to the 10 test images for CelebA-HQ: https://drive.google.com/file/d/1YzldvLWTaaB_C_ware7vYv2zTvSBL8HW/view?usp=sharing
