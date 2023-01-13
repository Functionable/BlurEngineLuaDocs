---
title: Log
summary: An enum
---


Used with the function `log`, it tells the engine the severity of your log message. It currently is only used to pick the color used for that message.

| LOG_ERROR <span style="float: right;">Constant: 2</span> |
| ------------------- |
| Yields a red background around the log subject |

| LOG_FATAL <span style="float: right;">Constant: 3</span> |
| ------------------- |
| Results in a slightly darker red around the log subject |

| LOG_INFO <span style="float: right;">Constant: 1</span> |
| ------------------- |
| Ends up being bright blue around the log subject |

| LOG_VERBOSE <span style="float: right;">Constant: 0</span> |
| ------------------- |
| Results in a slightly darker blue around the log subject than `LOG_INFO` |

| LOG_WARNING <span style="float: right;">Constant: 4</span> |
| ------------------- |
| Results in a yellow background around the log subject |

