# PyTorch-Summary
Keras style summary. Supports modular network structures e.g. layers organized into feature extraction and classification.

## Usage
```python
from summary import summary

# explict call
model_summary = summary(model = model, device = torch.device('cpu'), input_size =(1, 3, 224, 224), verbose = False)
model_summary.printer()

# implicit
model_summary = summary(model = model, device = torch.device('cpu'), input_size =(1, 3, 224, 224), verbose = True)

