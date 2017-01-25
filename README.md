# CSVideoNet

1. 0.25_196_ExtractFrame.sh is used to extract frames from videos.
2. generateTrainCNN.m is used to generate image blocks for training CNN1(Background CNN).
3. "caffe/model/crX" directory contains all the necessary file for training CNN1.
4. extractFeatures_5_25.m is used to extract the intermediate feature extracted by CNN1. 
5. "model" directory contains all the files for training the whole framework. The pre-trained CNN1 is loaded, further trained with the whole framework using the intermediate feature as input. The original image blocks is the input for training CNN2, CNN2 is trained from scratch. 
6. Run VideoNet.lua to train the whole framework.
