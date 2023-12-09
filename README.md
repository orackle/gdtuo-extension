# Optimized Optimizer: Unveiling the Power of Gradient Descent 

### Original Paper

[NeurIPs 2022: Gradient Descent: The Ultimate Optimizer](https://proceedings.neurips.cc/paper_files/paper/2022/hash/36ce475705c1dc6c50a5956cedff3d01-Abstract-Conference.html)  

Authors: Kartik Chandra, Audrey Xie, Jonathan Ragan-Kelley, ERIK MEIJER

### Original Code: 

(Github Link)[https://github.com/kach/gradient-descent-the-ultimate-optimizer]

### How to run our code:

1. Download ipynb files - (sgd_on_streiods.ipynb to run our custom SGD, extending_datasets.ipynb to view results of original gdtuo against the CIFAR-100 and Iris datatsets)
2. Run it on Colab or local environment in VS Code
   
### Optimized Optimizer: Unveiling the Power of Gradient Descent 

This research extends gradient descent optimization by recursively stacking hyperparameters, inspired by Chandra et al. (2022). Our approach, implemented in PyTorch, demonstrates enhanced convergence, generalization, and adaptability across diverse datasets. Find the code at [GitHub](https://github.com/dghosh2/gdtuo-extension).

We have also extended the testing domain by testing against CIFAR-100 and Iris Datasets and reported our findings in our paper. 

Further, we have introduced new hyperparamaters in the original GDTUO's Ultimate_SGD's code:
- Dampening: This factor makes the optimization process smoother. It reduces the intensity of the updates made to the model’s parameters, providing stability and preventing drastic changes that might hinder convergence.

- Weight Decay: Weight decay (wd) helps control the size of the model’s parameters during the training process, preventing them from becoming too large, which can lead to overfitting. Overfitting occurs when a model performs well on training data but fails to generalize to new, unseen data

### Contribution

Omkar Shinde (oshinde1)
- Worked on modifying the gdtuo code and creating SGD_ON_STEROIDS
- Tested stacking multiple hyperoptimizers and the accuracy of SGD_ON_STEROIDS 

Debangana Ghosh (dghosh2)
- Worked on replicating original code and comparing against standard pytorch optimizers
- Tested gdtuo and recursive optimizers performances on CIFAR-100 and Iris datasets
  
### Acknowledgments

We express our sincere thanks to Chandra et al. for creating the gdtuo optimization library. Their work has notably advanced optimization in machine learning, showcasing gdtuo's versatility across diverse datasets. The foundational principles they established have been crucial to our explorations in semi-supervised learning. Additionally, we are profoundly grateful to Professor Adnan Rakin for his supervision and guidance throughout this research. His insights and expertise have been instrumental in navigating the complexities of our work.
