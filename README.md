# Unet-2D-car-segmentation
This repository contains ipython implementation of U-net network for car segmentation in 2D based on grayscale or RGB color images. The training and test dataset are from carvana Kaggel challenge (144 images and 144 ground-truth masks). The model has been tested on Linux and Windows 10. Using this example, good result can be achived with in a few minutes depending on number/type of the GPUs.

This implementation is based on Keras with Tensorflow backend. 

> It has been tested on Python 3.6, Anaconda (4.7). 
> The uplaoded code requires a GPU but if you do not have one, simply uninstall tensorflow-gpu (pip uninstall tensorflow-gpu), then install regular tensorflow (pip install tensorflow) and the code will work.


This can serve as an example for learning to:

  - **Train a network using your own images**
  
  - **Learn the structure of Unet netwrok**
  
  - **Test and fine tune a network to improve the segmentation task**
  
  - **Perform 2D segmentation with other datasets**


# Test
1. Unzip data folder
2. Create a virtual environment with Anaconda:  conda create -n DL_example python=3.6 (Python 3 is compatible with packages)
3. Activate the environment: activate DL_example
4. Change directory to where you cloned the current files: cd ./where files are downloaded
5. Install required libraries: pip install -r requirements.txt

To test the notebook version, type the following in the command line:  jupyter notebook
This will open the notebook which will allow you to run either the grayscale (car_segmentation_Unet_grayscale.ipynb) or RGB (car_segmentation_Unet_rgb.ipynb) version of the code. You should be able to run each cell and get the result.

# Test by Horace, 2021/09/15
1. Unzip data folder
2. Create a vritual environment with pyenv (i.e., pyenv virtualenv 3.6.5 unet_car)
3. Create a local environment (i.e., pyenv local unet_car)
4. Install required python packages (i.e., pip install -r requirements.txt)
5. Install tensorflow CPU version (i.e., pip install tensorflow)
6. Install jupyter notebook (i.e., pip install jupyter)
7. Start jupyter notebook (i.e., jupyter notebook)
![image](https://user-images.githubusercontent.com/55008636/133451570-564cf80e-8409-4ea8-bd9c-bd3db4505913.png)

8. Troubleshooting for "ModuleNotFoundError: No module named 'cv2'"
9. Install jupyter lab (i.e., pip3 install jupyterlab)
10. Revise the attached notebook with revise path and adam()

# Reference
Ronneberger, Olaf, Philipp Fischer, and Thomas Brox. "U-net: Convolutional networks for biomedical image segmentation." In International Conference on Medical image computing and computer-assisted intervention, pp. 234-241. Springer, Cham, 2015.

# License
The code comes "AS IS" with no warranty of any kind. It can be used for any educational and research purpose. Feel free to modify and/or redistribute.
