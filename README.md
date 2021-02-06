[![INFORMS Journal on Computing Logo](https://INFORMSJoC.github.io/logos/INFORMS_Journal_on_Computing_Header.jpg)](https://pubsonline.informs.org/journal/ijoc)

# On the Cluster-aware Supervised Learning (CluSL): Frameworks, Convergent Algorithms, and Applications

This archive is distributed in association with the [INFORMS Journal on
Computing](https://pubsonline.informs.org/journal/ijoc) under the [MIT License](LICENSE).

The software and data in this repository are a snapshot of the software and data
that were used in the research reported on in the paper 
[On the Cluster-aware Supervised Learning (CluSL): Frameworks, Convergent Algorithms, and Applications](https://doi.org/10.1287/ijoc.2020.1053) by S.T. Chen and W.J. Xie. 



## Cite

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4512367.svg)](https://doi.org/10.5281/zenodo.4512367)

To cite this software, please cite the [On the Cluster-aware Supervised Learning (CluSL): Frameworks, Convergent Algorithms, and Applications](https://doi.org/10.1287/ijoc.2020.1053) using its DOI and the software itself, using the DOI.

Below is the BibTex for citing this version of the code.

```
@article{CluSL,
  author =        {S.T. Chen and W.J. Xie},
  publisher =     {INFORMS Journal on Computing},
  title =         {{CluSL} Version v2020.1053},
  year =          {2020},
  doi =           {10.1287/zenodo.4512366},
  url =           {https://github.com/INFORMSJoC/2020.1053},
}  
```

## Description

The files provided in this respository are the online supplement to the paper *On the Cluster-aware Supervised Learning (CluSL): Frameworks, Convergent Algorithms, and Applications.* Three subdirectories: *src*, *data* and *results* are shown here. *src* contain the source code used in all experiments in this paper. *data* contain data files needed for experiments. *results* contain the raw results from the paper as well as all figures. Two frameworks (algorithms) are proposed in this paper, yielding eight experiments (Experiment 1-6 for the first one, Experiment 7-8 for the second one) in three subdirectories respectively. To successfully run the code in subdirectories, you may need to install Python (i.e. .py files) and Matlab (i.e. .m files). The paths used to process the data in the codes should be revised accordingly.

 Below is the detailed explanation.

## Input Data
*data/Experiment 1*

The data file contains nine sets of hypothetical data generated using the given distribution displayed in the paper. Sheet1-Sheet3, Sheet4-Sheet6, Sheet7-Sheet9 include three sets of one-dimensional, two-dimensional, and three-dimensional data points correspondingly, where the last column of each sheet is regarded as the response variable.

*data/Experiment 2*

Hypothetical data was generated using a piece-wise function explained in the paper. The data file includes 500 training data points and 9 testing datasets (500 data points each).

*data/Experiment 3*

Three files contain datasets used in real estate valuation, red wine, and white wine quality cases. The source data are available at https://archive.ics.uci.edu/ml/index.php.

*data/Experiment 4*

The "housing.csv" used in Experiment 4 contains 20640 data points with 9 features. Data cleaning should be implemented according to the paper. More detailed information is available at [https://www.kaggle.com/camnugent/California-housing-prices](https://www.kaggle.com/camnugent/California-housing-prices)

*data/Experiment 5*

Five files contain datasets used in "Contraceptive Method Choice", "Steel plates faults", "Wireless indoor localization", "White wine quality 5 classes", and "Yeast" cases. The source data are available at https://archive.ics.uci.edu/ml/index.php. Please note that in the white wine case, we removed level 3 and 9 which contain very few data.

*data/Experiment 6*

Three files contain three datasets used in "CIFAR-10", "Magnetic-tile-defect", and "MNIST handwritten digits" cases. Please note that we preprocessed the second dataset images by uniformly resizing all the images into 50×50 pixels. The source data are available at [http://www.cs.toronto.edu/~kriz/cifar.html](http://www.cs.toronto.edu/~kriz/cifar.html)
[https://github.com/abin24/Magnetic-tile-defect-datasets.](https://github.com/abin24/Magnetic-tile-defect-datasets.)  and http://yann.lecun.com/exdb/mnist/.

*data/Experiment 7*

"digital.xlsx" contains both the training and testing images in the "Semeion Handwritten Digit" case. The size of each image is 16×16 grayscale values. "training.xlsx" and "testing.xlsx" contains the training and testing images in the "Optical Recognition of Handwritten Digits" case. The size of each image is 8×8. The source data are available at https://archive.ics.uci.edu/ml/index.php.

*data/Experiment 8*

Please refer to Data Set Info in folder Experiment 6.
## Source code

*src/Experiment 1*

The code folder includes one .py file and one .m file. "Experiment 1. py" is the code of the first algorithm in the paper. "CluSL.m" is the Matlab code of solver Knitro.

*src/Experiment 2*

The code folder includes the .py file used for Experiment 2.

*src/Experiment 3*

The code folder includes three py files. "Experiment 3_RAM.py" is the code of the proposed algorithm in the paper. "Experiment 3_RF.py" and "Experiment 3_SVR.py" are open-sourced Random Forest and Support Vector Machine codes in the scikit-learn package.

*src/Experiment 4*

The code folder includes the .py file used for Experiment 4.

*src/Experiment 5*

The code folder includes two .py files. "Experiment 5_Clu-MSVM.py" is the code of the proposed algorithm in the paper. "Experiment 5_SVC.py" is an open-sourced Support Vector Classification code in the scikit-learn package.

*src/Experiment 6*

The code folder includes three .py files. "Experiment 6_Clu-CNN.py" is the code of the first algorithm in the paper. "Experiment 6_CNN.py" is an open-sourced Convolutional Neural Networks code in the Python deep learning API: Keras. "read_data.py" includes some preprocessing process of image data.

*src/Experiment 7*

The code folder includes two .py files. "Experiment 7_F-RAM.py" is the code of the second framework and algorithm in the paper. "Experiment 7_CNN.py" is open-sourced Convolutional Neural Networks code in the Python deep learning API: Keras.

*src/Experiment 8*

The code folder includes three .py files. "Experiment 8_FCluSL.py" is the code of the second framework and algorithm in the paper. "Experiment 8_CNN.py" is an open-sourced Convolutional Neural Networks code in the Python deep learning API: Keras. "read_data.py" includes some preprocessing process of image data.


## Results

*results/Experiment 1 - results/Experiment 8* contain the raw results from the paper as well as all figures.

