# music-generator

![Music Generator in Netlogo](images/screenshot_1.png)

This project consists of two simulations:

#### Notes.nlogo

A study to the emergent behavior of music notes. The tone stands for the current key of the simulation. for example: 

``` 
tone(60) = C
```

Whenever two notes collide, they will produce a sound if they form a valid combination in the current key. For example, suppose C and D collide when tone is 60. Since C and D are both in the scale of C, one of them will play its tone. when ```only_chords``` is on, only combinations that form a chord will be played. The sadness is a (to be honest: weak) isomorph for the scale. From sadness=0 to sadness=100 the scale is: ```maj, maj7, min, min7```.

#### Sequencer.nlogo

This simulation creates sequences of tones in a random ground-tone. After setup, x notes fly around at random through the world, making a sound and changing their direction when colliding. When adding the sequencer, a star will be added to the world, acting as the sequencer. The first note that collides with the sequencer will be the ground-tone of the composition.
every following colliding note that is part of the scale of the ground-tone will be added to the composition.

The user has the possibility to play around with the sequence by changing the tone, the instrument and the speed.
