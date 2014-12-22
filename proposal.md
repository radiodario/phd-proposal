# Research Proposal
Serialising Livecoding performances on an massively-online web platform.

## Introduction
Live coding is an art form. Be it a musical, or more recently, visual performance, these pieces entrhall and entertain audiences accross the world. The pieces themselves exist in their purest form only momentarily, while they are executed by the artist. As such, are usually are usually recorded as videos, effectively "freezing" them into a format that doesn't afford easy analysis.

Due to the relative infancy of live coding as an art form and the "raster" nature of the current preferred mode of storage, the study of these performances is practicaly limited to manual, ad-hoc work. However, code, the very medium used to create these pieces is inherently serialisable. While many artists divulge the results of these performances online as code, they lack a key aspect: a representation of the process undergone by the artist when creating the piece.

By recording the code and keystrokes inserted by the performers as they play, we enable these pieces to be stored and replayed in an interactive manner. This in turn would allow for analysis and evaluation, encouraging the creation of derivative works. Furthermore, the ability to formally study and analyse the process of these artists would enable more potential live coders to learn from more adept artists, as well as gaining insights on the nature of this novel artform.

We propose the creation of a platform that would combine the performance ability of environments such as SuperCollider or Livecodelab, but in an online manner, so that performances could be broadcast and enjoyed *live* without needing to be in the same physical space as the performer.

It is expected that this platform would also encourage collaboration between artists. Once the system is built, it would be trivial to create a multi-performer mode, so that more than one artist could have input at a given time. By making the system opensource, it is expected that the collaborative nature of the live coding scene would encourage other individuals to improve and create more modes - perhaps allowing for competitive "laptop battles" happening online for thousands to witness, enjoy and learn from.

## Research Questions
* Creating a technique to serialise, store and broadcast livecoding performances to an audience as they are performed, storing them on a server and executing them locally as they are received.
* How would the replayability and transparency of a live coding piece help lower the high entry barrier to live coding. Can an online platform help others learn how to livecode more effectively?
* Are there any common patterns on live coding performances that can be identified? Are there different *schools* or *styles* that can be quantitatively identifed? Could this online platform help create and spread these styles?

## Process
There are currently several open-source web live coding environments  which a great number of artists are already familiar with. Leveraging these systems, the platform would integrate a websockets system to connect several instances of these livecoding environments, in either *performer* or *audience* form.

The server orchestrating the performance, relaying the keystrokes and code changes to the all of the clients, would also be in charge of storing these; and on demand, it would allow for retrieval of the piece by a client at any point, usually by calling on a known url route.

One of the major hurdles to overcome in order for this platform to work would be the creation of a format that efficiently captures the actions of the performer, while remaining lightweight.

## References

1. Supercollider - http://www.audiosynth.com/
2. LiveCodeLab - http://livecodelab.net/