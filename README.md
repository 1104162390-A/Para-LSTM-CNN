# Wearable Electronic Glove and Multi-layer Parallel LSTM-CNN based Method for Sign Language Recognition.
In this git repository a Para-LSTM-CNN algorithm based on parallel features extraction strategy is proposed. The temporal and spatial features of the sensor signals are extracted through long short-term memory (LSTM) and convolutional neural network (CNN), respectively. The Para-LSTM-CNN can effectively improve the accuracy of sign language recognition by fusing spatial and temporal features synchronously.

If you're using our code, please cite our paper (available on https://...):

 (High-definition frame diagram image of the Para-LSTM-CNN will be updated )


![proposed Architecture](https://github.com/1104162390-A/Para-LSTM-CNN/blob/main/Para-Struture_of_LSTM-CNN.png)

we have added codes for models that we tested:
- Para-LSTM-CNN model 

## Setup

`pip3 install -r requirements.txt`

## Guide to run the code

1. The data for the subjects resides in the `data` directory. You can create subdir for the arrangement and the dataset.npy file as `data/arrangement/dataset.npz`. We used the processed data from [here](https://github.com/arturjordao/WearableSensorData/tree/master/data) and put it in the data folder. For example: 'data/LOTO/MHEALTH.npz' file depicts the leave one trial out (LOTO) for the MHEALTH dataset. 

2. The codes reside in the  `codes` folder. 
* `codes/model_baseline`: This folder contains the Python code for training a baseline model containing CNN and RNN layers. You can run the code by running the following command:
```
python3 model_baseline.py
```

* `codes/model_proposed`: This folder contains the Python code for training the proposed model built using Keras and Tensorflow. Self-attention was coded from [here](https://github.com/uzaymacar/attention-mechanisms). You can run the code by running the following command:

```
python3 model_with_self_attn.py
```

