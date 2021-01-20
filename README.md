# 3dAssets

| Format | iOS (ARkit3) |  Android (ARCore) | PBR |  Type | Convert from | Convert to | Editor | Comment
| ------ | ------ |  ------ | ------ | ------ | ------ | ------ | ------ | ------ |
| .SCN | :white_check_mark: | :x: | :white_check_mark: | Binary | dae,usd,abc,obj | non | Xcode | Xcode.3D+textures  
| .OBJ | :white_check_mark: | :white_check_mark: | Possible | coordinates | 3DP | scn | any | can direct import/export from some 3D programs. 3D with seperate texture folder. manually apply / editing MTL file  to read PBR information is possible but this format do not support animation. 
| .DAE | :white_check_mark: | :white_check_mark: | :x: | XML | 3DP | scn | any | can direct import/export from some 3DP = 3D programs. 3D with seperate texture folder. manually apply all links in scenekit and scenekit will forced to save as scn file |  
| .USDZ | :white_check_mark: | :x: | :white_check_mark: | zip but not compressed | TEP | Xcode  | N/A | direct export by a TEP texture editing program only atm. 3D+textures 
| .USDA | :white_check_mark: | :x: | :white_check_mark: | ASCII| USDC | USDZ/C | Xcode | intermediate file convert from USDC. 3D+textures 
| .USDC | :white_check_mark: | :x: | :white_check_mark: | binary | TEP | USDA/Z| N/A | directly exported along with usdz file from source TEP texture editing program only atm. 3D+textures |
| .GLB | :x: | :white_check_mark: | :white_check_mark: | compressed | GLTF | N/A |N/A | can direct output from some 3D programs. 3D+textures |
| .GLTF | :x: | :white_check_mark: | :white_check_mark: | JSON  | any | USDZ/A only |any |  can direct output from any 3D programs. 3D+textures |
| .FBX | :x: | :white_check_mark: | :x: | ASCII/binary  | 3DP| N/A |  N/A | N/A | 3DP = 3D program
| .ABC | :white_check_mark: | :x:  | :white_check_mark: | binary | 3DP | N/A| N/A | too big of file size, suitable for animation but not for 3D mesh static assets atm