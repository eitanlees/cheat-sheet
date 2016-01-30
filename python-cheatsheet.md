Python Cheatsheet
=================

General
-------

### Makeing empty lists

```python
fouremptylists = [[] for __ in xrange(4)]
```


Pickel
------

### pickel.dump

```python
import pickle
favoritecolor = { "lion": "yellow", "kitty": "red" }
pickle.dump( favoritecolor, open( "save.p", "wb" ) )
```

### pickel.load

```python
favoritecolor = pickle.load( open( "save.p", "rb" ) )
```

OS
--

### Making the system speak (OSX)

```python
os.system("say 'hello world'")
```

I/O
---

### Writing csv with numpy.savetxt [man](http://docs.scipy.org/doc/numpy/reference/generated/numpy.savetxt.html)
```python
np.savetxt('output.dat', np.column_stack(results), header = 'My Results', delimiter = ",")
```

Jupyter
-------

```python
%matplotlib inline
%config InlineBackend.figure_format = 'svg'
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```
