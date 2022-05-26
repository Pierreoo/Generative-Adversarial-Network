# Generative-Adversarial-Network

Generation of 10k rows of new data from the same distribution <br>

Simple Method 1 represents the initial idea to make use of statistics for generating new data. As the column features could be generalized by a multivariate normal distribution, new samples could be produced by making use of the means and covariance between columns. However, this induces a shift as illustrated by comparing Figure 1 and 2.

Therefore, the implementation of a GAN or VAE is preferred for data augmentation. The goal of Advanced Method 2 is to construct plausible row vectors with thus coherent column features. The implementation of a GAN promotes diversity to mimic the original dataset distribution.

Inspiration for the GAN network was found on: RealPython GAN. The latter resource was useful to distinguish this use case from image data. In addition, as optimization is hard to define given the data, the best outlook is to assess the generator by visually comparing Figure 1 and 3. Therefore, dropout and a low learning rate was necessary as a regularization technique to avoid overfitting.

The 10k rows of new data is represented by generated_samples in the notebook.
