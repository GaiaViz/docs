---
title: Animation - Channels and Tracks
layout: home
nav_order: 
parent: Tutorials and demos
---

In theory, current constants set to support:

1 million ch-map rows (track -> attribute mappings).
   10 million node properties updated (per frame).

1 million tracks (columns).
108000 samples per track (rows) = 30min at 60Hz.

750M total track samples (track columns X track rows), uses 3GB RAM.

Here is a (reminder) link to the channel/track key functionality:
[https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#animation---channels--tracks](https://github.com/GaiaViz/GaiaViz/wiki/User-Commands#animation---channels--tracks)

-----
working on the numbers.. been adjusting the constants and testing.. best guess stats:

30 minutes at 60fps (max of 108000 samples per track)
1 million attribute mappings (track -> node attribute)
10 million properties assigned (eg. 1M nodes w/ 10 properties mapped, multiple nodes sharing channel(s))

*best guess = not tested, (largest test just now was 319 tracks with 36k samples).
  - note that the ver from Sat is fixed at 7200 samples = 2min.  

i would add that i fixed some bugs, but disabled the rolling file buffer (hence 108K samples vs infinite) and OSC -> track methods (so reads from file only at this point).. however, with a little work both could be turned back on (no limit to number of track samples) and live track data via OSC.

----
