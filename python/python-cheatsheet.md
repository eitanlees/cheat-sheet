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

### Making the system speak

```python
os.system("say 'hello world'")
```
