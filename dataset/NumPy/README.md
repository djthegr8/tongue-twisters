## NumPy format
Due to the increasing usage of `.npy` files, the tongue twwister dataset is available in that format too.
                               
The usage of this file is easy using NumPy.       
#### Usage
To use this, simply import it into your workspace, script or Jupyter notebook, which may look like the below in Python.
```py
import numpy as np
tongue_twisters = np.load('database.npy', allow_pickle=True)
```

