---
title: Sound
summary: A BlurLua class
---


A sound that can spawn multiple instances of itself

## Properties
| **number** Pitch |
| --------------------- |
| Pitch of the sound     |

| **number** Volume |
| --------------------- |
| Volume of the sound (0-1)     |

| **bool** Loop |
| --------------------- |
| Details whether the sound should loop     |

| **number** Pan |
| --------------------- |
| -1 being left only, and 1 being right only, pans the sound.     |

## Functions
| Sound:stopAll(  )  |
| ------------------- |
| Stops all active SoundInstances |



| **SoundInstance** Sound:play(  )  |
| ------------------- |
| Plays a sound, and creates a new SoundInstance |



