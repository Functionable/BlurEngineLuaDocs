---
title: SoundInstance
summary: A BlurLua class
---


An individual instance of a sound that can be controlled

## Properties
| **bool** Paused |
| --------------------- |
| If enabled, allows for the sound to be stopped temporarily     |

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
| SoundInstance:stop(  )  |
| ------------------- |
| Stops the specific SoundInstance |



| SoundInstance:isPlaying(  )  |
| ------------------- |
| Returns false if the object stopped playing of if `Paused` equals `true`. If `Paused` is `false` and `isPlaying` returns `false`, you must create a new SoundInstance in order to start playing the audio again. |



