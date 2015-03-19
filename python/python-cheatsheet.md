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

### Writing csv with numpy
```python
np.savetxt('output.dat', np.column_stack(results), header = 'My Results', delimiter = ",")
```
