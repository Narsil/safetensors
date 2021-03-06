## Installation

```
pip install safetensors
```


## Usage

### Numpy

```python
from safetensors.numpy import save_file, load_file
import numpy as np

tensors = {
   "a": np.zeros((2, 2)),
   "b": np.zeros((2, 3), dtype=np.uint8)
}

save_file(tensors, "./out.bin")


# Now loading
loaded = load_file("./out.bin")
```

### Torch

```python
from safetensors.torch import save_file, load_file
import torch

tensors = {
   "a": torch.zeros((2, 2)),
   "b": torch.zeros((2, 3), dtype=torch.uint8)
}

save_file(tensors, "./out.bin")


# Now loading
loaded = load_file("./out.bin")
```
