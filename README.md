# WHOI-ML: About This Repository
This Repository contains notes, resources, and assignments for a Machine Learning Bootcamp for the Woods Hole Oceanographic Institution.

# About This Document
This ReadMe outlines the content of the bootcamp, provides installation instructions for the required software packages, and suggests background reading material for extended study.

# Course Structure
The course will run over 3 days in six 4-hour sessions. Each session will be broken up into 3-4 subsections consisting of presentation content and a practical component. Practical components are designed so that the minimal learning goals can be comfortably met within the allotted time, but stretch goals will allow participants to gain additional practice and deepen their understanding.

The six sections are:
1. **The Machine Learning Pantry** - Machine Learning comes in several different flavors (supervised, unsupervised, reinforcement, etc.) and there are several ready-made libraries that will give us 80% of the functionality in 20% of the time. In this section, you will use scikit-learn and matplotlib to make predictions.
2. **Neural Networks and Supervised Training** - Artificial Neural Networks have been used to great effect in almost every area of machine learning, thanks to their flexibility, their simplicity of use, and the explosion of available training data. In this section you will use pytorch to define and train several types of neural networks to solve several types of machine learning problem. Although why they work is still something of a mystery, this section will elucidate when they work, and what to try when they don't.
3. **Structured and Spatio-Temporal Data** - Data often have structure that constrains what is possible or what is likely. In this section, you will learn to use clustering algorithms on discrete spatial categories, represent continuous functions using Gaussian Processes, represent sequential and temporal data, and encode translational symmetry using convolutional structures.
4. **Unsupervised Learning and Anomaly Detection** - Unsupervised (and self-supervised) techniques can be used to summarize data, providing interpretability, computational simplification, and measures of typicality. In this section, you will use PCA, t-SNE, and mixture models to summarize data, and you will use data reconstruction error and likelihoods to identify outliers.
5. **Reinforcement Learning and Automation** - Machine Learning can be used to optimize decisions and improve them over time. In this section you will apply several versions of Thompson Sampling to decision problems with uncertainty, and you will apply REINFORCE to decisions with long-term effects.
6. **Machine Learning in the Real World** - In this section you will apply what you've learned to a dataset of your choice. This section will also describe some approaches to scalability, addressing time, memory, and data constraints.

# System Requirements
Any machine with an up-to-date popular desktop operating system (Mac OS, Windows, Ubuntu, e.g.) and a modern web browser installed will be sufficient for this course. That said, machine learning can be computationally intensive, so higher-end CPU's will save time, and machines with NVidia GPUs _may_ be able to leverage them for faster training of neural networks, in the section of the course pertaining to that. However, modest hardware will still be sufficient for the purpose of the course.

# Software Packages
This program uses many software packages, but fortunately will only require two installs, as a large number of the packages we will use come packaged with Anaconda.  
1. [Install Anaconda](https://www.anaconda.com/distribution/). If offered a choice, download and install the package with the most recent version of Python (3.7). Anaconda is a scientific computing package that bundles many software packages and libraries we will be using in the course, including Python, Jupyter Notebooks, the conda package manager, matplotlib, numpy, pandas, scikit-learn, tqdm, and many more.
2. [Install PyTorch](https://pytorch.org/). PyTorch is a deep-learning library (comparable to Tensorflow) with a shallow learning curve and high flexibility. This is easiest to do through the command line, using the conda package manager. In the "Getting Started" section, you can choose the install command that fits your environment. Note that if you are not running on a CUDA-supported NVidia GPU, you should choose "none" to install only the CPU version of PyTorch. Windows users may need to run the installation command through Power Shell or by going through Anaconda Navigator > Environments > base (root) > Open Terminal.
3. Test the installation by opening a new Jupyter notebook and running  
`import torch`  
`print(torch.__version__)`    
Jupyter notebooks can be opened by either running `jupyter notebook` from a shell/terminal or by going through the Anaconda Navigator > Jupyter Notebooks. Either option should open a page in your web browser that will allow you to browse files and create a new notebook by clicking new > Python 3. Type the code above into a cell, and then execute the cell by pressing Shift+Enter.

# Background Reading:
No prior knowledge of Machine Learning is assumed in this course, but a strong programming background is assumed. The course will be exclusively in Python, and participants may want to review some of the following pages so that they can focus exclusively on Machine Learning once the course begins.  
- [Python Cheat Sheet](https://perso.limsi.fr/pointal/_media/python:cours:mementopython3-english.pdf). Feel free to search or follow a tutorial if anything needs clarification.
- [Python Classes/Objects](https://www.w3schools.com/python/python_classes.asp)
- [Python Special Methods](https://micropyramid.com/blog/python-special-class-methods-or-magic-methods/) (`__init__`, `__str__`, `__repr__`, etc.). There is a gentler introduction [here](https://dbader.org/blog/python-dunder-methods).
- [Functional Programming](https://kite.com/blog/python/functional-programming/)
- [Debugging in Python](https://realpython.com/python-debugging-pdb/). Although Jupyter notebooks make interactive programming and introspection through `print` statements very flexible, `pdb` may still be useful to developers aiming at 10x engineer status.

# Additional Resources:
These resources will not be used in this course, but those hoping to explore some areas in greater detail may find them worth looking into.

### Troubleshooting Neural Networks
- Josh Tobin - [Troubleshooting Deep Neural Networks](http://josh-tobin.com/troubleshooting-deep-neural-networks.html)
- Andrej Karpathy - [A Recipe for Training Neural Networks](http://karpathy.github.io/2019/04/25/recipe/)
    - See also: Karpathy's [tweet thread](https://twitter.com/karpathy/status/1013244313327681536) on common neural net mistakes
- Matt Holt & Daniel Ricks - [Practical Advice for Building Deep Neural Networks](https://pcc.cs.byu.edu/2017/10/02/practical-advice-for-building-deep-neural-networks/)

### Parallel/Distributed Training
- Thomas Wolf - [Training Neural Nets on Larger Batches: Practical Tips for 1-GPU, Multi-GPU & Distributed Setups](https://medium.com/huggingface/training-larger-batches-practical-tips-on-1-gpu-multi-gpu-distributed-setups-ec88c3e51255)

### Recurrent Networks
- Andrej Karpathy - [The Unreasonable Effectiveness of Recurrent Neural Networks](http://karpathy.github.io/2015/05/21/rnn-effectiveness/)

### Reinforcement Learning
For those interested in doing more reinforcement learning experiments (on Markov Decision Processes, not Bandit Problems), the libraries `gym` and `simple_rl` may be helpful. These can be installed through a python package manager, such as `conda` or `pip`.

### Other Courses
- fast.ai - [Practical Deep Learning for Coders](https://course.fast.ai/index.html)
- Stanford - [Convolutional Neural Networks for Visual Recognition](http://cs231n.github.io/)

# License Information
All content in this repository is ©2019 (S)am. It has been made available for educational purposes, but copying or redistributing this content is not permitted. If you would like to suggest changes to this repository or correct errors, please contact the owner of this repository or submit a pull request.
