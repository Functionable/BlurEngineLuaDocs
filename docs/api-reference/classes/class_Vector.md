---
title: Vector
summary: A BlurLua class
---


A vector helper class, with some math functions to make your life easier

## Properties
| **number** Y |
| --------------------- |
| Z dimension component     |

| **number** X |
| --------------------- |
| X dimension component     |

| **number** Z |
| --------------------- |
| Y dimension component     |

## Functions
| **number** Vector:magnitude(  )  |
| ------------------- |
| Calculates the magnitude of the vector |



| **Vector** Vector:abs(  )  |
| ------------------- |
| Returns a new vector with all it's components being absolute values of this vector's components |



| **Vector** Vector:normalize(  )  |
| ------------------- |
| Returns a normalized vector |



| **Vector** Vector:min( **Vector** otherVector )  |
| ------------------- |
| Returns a new vector with each of the components being the lowest from this vector and `otherVector` |



| **Vector** Vector:max( **Vector** otherVector )  |
| ------------------- |
| Returns a new vector with each of the components being the highest from this vector and `otherVector` |



