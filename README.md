# Capsule Network

---
The model contains the following libraries and frameworks
- Tensorflow 2.3
- Matplotlib
- tqdm
- numpy
---
  
The notebook CapsuleNetwork-50-epochs.ipynb notebook shows a training log for 50 epochs. However, weights for a model trained up to 100 epochs are stored in logs/model. The training logs of the remaining 50 epochs of the model are not shown in the notebook as they are trained during a different session using the checkpointed weights for the first 50 epochs. The model is checkpointed every 10 epochs giving us a total of 10 checkpoints. The `capsule-10` are the weights generated after training for 100 epochs. 

---

VisualizingCapsnetFeatures.ipynb notebook used checkpointed weights to visualize the features and some sample images are stored in the featureVisualization directory. You can simply just run this notebook and see the features for yourself.
