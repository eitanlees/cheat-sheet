Python Cheatsheet
=================

General
-------

### Makeing empty lists

```python
fouremptylists = [[] for __ in xrange(4)]
```

### Dictionaries
```python
>>> d = {'key':'value'}
>>> print(d)
{'key': 'value'}
>>> d['mynewkey'] = 'mynewvalue'
>>> print(d)
{'mynewkey': 'mynewvalue', 'key': 'value'}
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

### Standard Header Cell
```python
%matplotlib inline
%config InlineBackend.figure_format = 'svg'
import numpy as np
import matplotlib.pyplot as plt
```

### Automatic reloading magic:
```python
%load_ext autoreload
%autoreload 2
```


Matplotlib
----------

### Legend outside of plot
```python
plt.legend(loc='center left', bbox_to_anchor=(1, 0.5))
```

### Loop for subplots
```python
import matplotlib.pyplot as plt
import numpy as np

x = np.arange(11)
y = np.random.rand(len(x), 9)*10

fig, axes = plt.subplots(3,3, sharex=True, sharey=True)

for i, ax in enumerate(axes.flatten()):
    ax.bar(x, y[:,i], color=plt.cm.Paired(i/10.))

plt.show()
```
