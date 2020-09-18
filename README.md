# Paper abstract

Current approaches involve deep learning in solving an **image inpainting** task. We propose a **meta-algorithm** in which we can set a **probabilistic distribution** on images. The set distribution can be a **classic** one, e.g. **Normal** distribution, or a **modern** one, e.g. **PixelCNN++**. Our **first observation** is relatively unexpected: if a learnt distribution **generates** reasonable images, then this does not make it is a good candidate for **inpainting** via our proposed algorithm and vice-versa (if a learnt distribution gives reasonable results on image inpainting via our algorithm, then this does not make it is a good candidate for sampling a new image). Our **second observation** is that although the visual results of the state-of-the-art method are superior to ours, the training time for our method is lower. Hence, one can experiment faster with our method to see, for example, if the desired inpainting is learnable. Moreover, using a specific distribution, our algorithm **can be trained also on high-quality RGB images, like 1024 times 1024 pixels**. As for the experiments, we included visual results.

# Index words

Image inpainting, Probabilistic Machine Learning, Normal Distribution, Matrix Normal Distribution, PixelCNN

## Others

**Link to my trained models** (the archive is downloaded implicitly when needed if you use the notebook): https://drive.google.com/file/d/1ZPCSyBjaFV0Xo_onnx1K49MyxJDlbVKn/view?usp=sharing

**Link to testing images for CelebA-HQ 1024x1024** (the archive is downloaded implicitly when needed if you use the notebook): https://drive.google.com/file/d/11XKSCbFn0rs82xFyl0gtN-pHo3ipZbwc/view?usp=sharing

# Code and demo

## For mle-inpainting-small-medium.ipynb: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aciobanusebi/clean-mle-inpainting/blob/master/mle_inpainting_small_medium.ipynb)

1. **Find and select the cell called "END OF CODE: RUN UP TO NOW (Ctrl + F8)".**

2. **Run the code below this cell (e.g, press Ctrl + F8).**

3. If you want to train a model and save a model to your Google Drive account, go to "Save models" and follow the instructions from there.

4. If you want to train a model and let it in memory, go to "Train a model" and follow the instructions from there.

5. If you want to sample images from a trained model (from my trained models ("web" option for *modelLocation*), from your Google Drive or from memory), go to "Sample" and follow the instructions from there.

6. **If you want to inpaint an image using a trained model (from my trained models ("web" option for *modelLocation*), from your Google Drive or from memory), go to "Test" and follow the instructions from there.**


## For mle-inpainting-large.ipynb: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/aciobanusebi/clean-mle-inpainting/blob/master/mle_inpainting_large.ipynb)

1. If you want to train a model and save a model to your Google Drive account, go to "Train" and follow the instructions from there.

2. **If you want to inpaint an image using a trained model (from my trained models ("web" option for *modelLocation*), from your Google Drive or from memory), go to "Test" and follow the instructions from there.**
