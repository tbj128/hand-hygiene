# Detecting Hand Hygiene Dispenser Use

### Background
- See: https://docs.google.com/document/d/1iPzdrs4tEbltL9iHykD_KKQxFjcWRBDu5fH6YkuxFFM/edit

### Approach
Due to limited number of samples, the main approach used transfer learning. The model consisted of the following layers:
- ResNet-50 base model
- ConvLSTM2D layer
- AvgPool
- Dense (128)
- Dropout (0.2)
- Dense (sigmoid)

### Results (best model)
- Train Accuracy: 95.8%
- Val Accuracy: 87.5%
- Trained over 29 epochs
