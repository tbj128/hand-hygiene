# Detecting Hand Hygiene Dispenser Use

### Background
- See: https://docs.google.com/document/d/1iPzdrs4tEbltL9iHykD_KKQxFjcWRBDu5fH6YkuxFFM/edit

### Approach
Due to limited number of samples, the main approach used transfer learning. The model consisted of the following layers:
- ResNet-50 base model
- ConvLSTM2D layer
- AvgPool
- Dense (sigmoid)

### Results
- Train Accuracy: 96.7%
- Val Accuracy: 80.4%
- Trained over 27 epochs
