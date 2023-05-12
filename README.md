# U-Net-in-PyTorch
This is an implementation of the U-Net model from the paper, [U-Net: Convolutional Networks for Biomedical Image Segmentation](https://papers.labml.ai/paper/1505.04597).

## How does it work?
U-Net is made up of a contracting path and an expanding path.
The contracting route is a series of convolutional layers and pooling layers that gradually diminish the resolution of the feature map.
The expansive route is a succession of up-sampling and convolutional layers that gradually enhance the resolution of the feature map.

The relevant feature map from the contracting path is concatenated with the current feature map at each step in the expansive path.

## Architecture
![image](https://github.com/Mostafa-wael/U-Net-in-PyTorch/assets/56788883/bf599396-011f-40d1-b053-f6d5f695a7d5)

## Example output
Image -> Mask -> Predicted Mask
![download](https://github.com/Mostafa-wael/U-Net-in-PyTorch/assets/56788883/7ea799cb-2830-4841-a12b-fba6d60cbe04)
>> Generated using this [test script](./test.py).

## Implementation 
Check the [attached notebook](./U_Net.ipynb) for implementation details. 


