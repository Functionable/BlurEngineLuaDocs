---
title: BLF Property Type
summary: An enum
---


This enum is used only in BLF definitions, when you have to specify where an attribute will be saved to

| BLF_ACCESSFUNCTION <span style="float: right;">Constant: 1</span> |
| ------------------- |
| TThis value indicates that the attribute, upon load, will funnel it's data to a getter/setter you can specify |

| BLF_ACCESSPROPERTY <span style="float: right;">Constant: 0</span> |
| ------------------- |
| This value indicates that the attribute, when loaded, should be plainly put into the output object table |

