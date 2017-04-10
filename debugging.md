### py.test

Modify the test module:

```python
import pytest
# set a breakpoint
pytest.set_trace()
```

Call the test with `--pbd` option:

```python
py.test --pdb unit_test.py
```

### ipython

```python
import ipdb; ipdb.set_trace()
```


### jupyter notebook

```python
from IPython.core.debugger import Tracer
Tracer()()
```
