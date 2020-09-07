# Capsule Network

## Requirements

The model contains the following libraries and frameworks
- Tensorflow 2.3
- Matplotlib
- tqdm
- numpy

---
## Pre-trained model
  
The notebook CapsuleNetwork-50-epochs.ipynb notebook shows a training log for 50 epochs. However, weights for a model trained up to 100 epochs are stored in logs/model. The training logs of the remaining 50 epochs of the model are not shown in the notebook as they are trained during a different session using the checkpointed weights for the first 50 epochs. The model is checkpointed every 10 epochs giving us a total of 10 checkpoints. The `capsule-10` are the weights generated after training for 100 epochs. 

## Training

For training the models yourself, simply delete the logs directory and run the CapsuleNetwork-50-epochs.ipynb notebook. Change the number of epochs (Default is 50).

The graph, loss and accuracy metrics are logged in ./logs folder and the model is checkpointed as discussed above.

![Tensorboard Graph](https://github.com/dedhiaparth98/capsule-network/blob/master/CapsuleNetwork-Tensorboard.png)

_**Note:** On running tensorboard yourself you may find the graph looking a bit different. To achieve same results add the gradients and reconstruction to the main graph and remove all read/write variables from the main graph_


---
## Visualizing Features

VisualizingCapsnetFeatures.ipynb notebook used checkpointed weights to visualize the features and some sample images are stored in the featureVisualization directory. You can simply just run this notebook and see the features for yourself with the weights my model is trained on. Incase you have trained it yourself, you could just change the checkpoint path.
