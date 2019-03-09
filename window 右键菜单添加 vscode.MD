我最终想要的效果如上图所示： 
- 右键文件夹，可以使用vscode打开 
- 右键单文件，可以使用vscode打开 
- 右键空白处，可以使用vscode打开

1. 新建一个"vsCodeOpenFolder"文件，复制如下代码，将一下路径修改为自己vsCode的路径,然后将文件后缀修改为".reg",双击运行vsCodeOpenFolder.reg,如果遇到弹出点是



Windows Registry Editor Version 5.00   
   
; Open files   
[HKEY_CLASSES_ROOT\*\shell\Open with VS Code]   
@="Edit with VS Code"   
"Icon"="F:\\ruanjiananzhuang\\qdsoftwork\\Microsoft VS Code\\Code.exe,0"   
   
[HKEY_CLASSES_ROOT\*\shell\Open with VS Code\command]   
@="\"F:\\ruanjiananzhuang\\qdsoftwork\\Microsoft VS Code\\Code.exe\" \"%1\""   
   
; This will make it appear when you right click ON a folder   
; The "Icon" line can be removed if you don't want the icon to appear   
   
[HKEY_CLASSES_ROOT\Directory\shell\vscode]   
@="Open Folder as VS Code Project"   
"Icon"="\"F:\\ruanjiananzhuang\\qdsoftwork\\Microsoft VS Code\\Code.exe\",0"   
   
[HKEY_CLASSES_ROOT\Directory\shell\vscode\command]   
@="\"F:\\ruanjiananzhuang\\qdsoftwork\\Microsoft VS Code\\Code.exe\" \"%1\""   
   
   
; This will make it appear when you right click INSIDE a folder   
; The "Icon" line can be removed if you don't want the icon to appear   
   
[HKEY_CLASSES_ROOT\Directory\Background\shell\vscode]   
@="Open Folder as VS Code Project"   
"Icon"="\"F:\\ruanjiananzhuang\\qdsoftwork\\Microsoft VS Code\\Code.exe\",0"   
   
[HKEY_CLASSES_ROOT\Directory\Background\shell\vscode\command]   
@="\"F:\\ruanjiananzhuang\\qdsoftwork\\Microsoft VS Code\\Code.exe\" \"%V\""
F:\\ruanjiananzhuang\\qdsoftwork\\Microsoft VS Code\\Code.exe,0"   
   
[HKEY_CLASSES_ROOT\*\shell\Open with VS Code\command]   
@="\"F:\\ruanjiananzhuang\\qdsoftwork\\Microsoft VS Code\\Code.exe\" \"%1\""   
   
; This will make it appear when you right click ON a folder   
; The "Icon" line can be removed if you don't want the icon to appear   
   
[HKEY_CLASSES_ROOT\Directory\shell\vscode]   
@="Open Folder as VS Code Project"   
"Icon"="\"F:\\ruanjiananzhuang\\qdsoftwork\\Microsoft VS Code\\Code.exe\",0"   
   
[HKEY_CLASSES_ROOT\Directory\shell\vscode\command]   
@="\"F:\\ruanjiananzhuang\\qdsoftwork\\Microsoft VS Code\\Code.exe\" \"%1\""   
   
   
; This will make it appear when you right click INSIDE a folder   
; The "Icon" line can be removed if you don't want the icon to appear   
   
[HKEY_CLASSES_ROOT\Directory\Background\shell\vscode]   
@="Open Folder as VS Code Project"   
"Icon"="\"F:\\ruanjiananzhuang\\qdsoftwork\\Microsoft VS Code\\Code.exe\",0"   
   
[HKEY_CLASSES_ROOT\Directory\Background\shell\vscode\command]   
@="\"F:\\ruanjiananzhuang\\qdsoftwork\\Microsoft VS Code\\Code.exe\" \"%V\""
