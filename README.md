Prerequisites
Pyhton（3.7）
Tensorflow（1.13.1）(an open source software library for high performance numerical computation https://pypi.org/project/tensorflow/)
Keras（2.2.4）（the Python deep learning API https://keras.io/）
Scikit-learn（0.24）（Free software machine learning library for Python programming language https://scikit-learn.org/stable/）
PyCharm（A professional Python IDE https://www.jetbrains.com/pycharm/）
Anaconda（1.9.7）(An open source Python distribution， https://www.anaconda.com/)
CUDA（10.0.130）（Computing platform launched by graphics card manufacturer NVIDIA https://developer.nvidia.com/cuda-toolkit-archive）
Cudnn（7.0）（GPU accelerated library for deep neural networks https://developer.nvidia.com/rdp/cudnn-archive）
Among them, Tensorflow is equipped with a GPU version, which can use GPU for accelerated calculations, and needs to match with CUDA and Cudnn.（See for details https://docs.nvidia.com/cuda/cuda-toolkit-release-notes/index.html）


Most of the dependencies can be installed through pip install with version number, e.g.
pip install tensorflow==1.13.1


File Description:
1*EBVData: The folder for storing data. There are two files, dsVIS_Data and VISDB_Data.
dsVIS_Data:
The positive data dsVIS_pos_Data.mat with a size of 2663×2000 and the negative data dsVIS_neg_Data.mat with a size of 26630×2000, each row of which is one piece of data.
VISDB_Data:
The positive data VISDB_pos_Data.mat with a size of 1104×2000 and the negative data VISDB_neg_Data.mat with a size of 11040×2000, each row of which is one piece of data.
2*Model: Store the trained DeepEBV model

3*Test_result: used to store model test results

4*EBVDataProcessing.py: This is a program dedicated to data processing, which takes all data to one_ Hot coding.

5*DeepEBV.py: This is the main program, including model creation, loading and testing

Run: 
1*Run first EBVDataProcessing.py After data encoding, dsVIS_Test_Data.npy, dsVIS_Test_Label.npy, VISDB_Test_Data.npy and VISDB_Test_Label.npy files will be generated and stored in ebvdata folder 
2* Run after DeepEBV.py, At the end of the run, the test results will be stored in test_ Results folder.
