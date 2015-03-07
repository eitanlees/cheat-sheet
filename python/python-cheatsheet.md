Python Cheatsheet
=================

General
-------

### Makeing empty lists

fouremptylists = [[] for __ in xrange(4)]


Pickel
------

### pickel.dump

import pickle
favoritecolor = { "lion": "yellow", "kitty": "red" }
pickle.dump( favoritecolor, open( "save.p", "wb" ) )

### pickel.load

favoritecolor = pickle.load( open( "save.p", "rb" ) )
