# Content

!!! warning
    This library is deprecated and it is likely it won't exist in future versions of BlurEngine.

## include

!!! info
    This function was `content.loadScript` prior to the removal of the `content` library.

Loads the script from *scripts / filePath* and executes it

| Parameter | Type   | Description                     | Example        | Required |
| --------- | ------ | ------------------------------- | -------------- | -------- |
| filePath  | string | Path of the lua script to load  | "script2.lua"  | yes      |

## texture.load

!!! info
    This function was `content.loadTexture` prior to the removal of the `content` library.

Loads a texture from `content/`*`filePath`*, and then returns it.

| Parameter | Type   | Description                 | Example        | Required |
| --------- | ------ | --------------------------- | -------------- | -------- |
| filePath  | string | Path of the texture loaded  | "crate.png"    | yes      |

| Returned | Type    | Description        | Example          |
| -------- | ------- | ------------------ | ---------------- |
| texture  | Texture | The loaded texture |                  |
