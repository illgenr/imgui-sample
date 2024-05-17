# Sokol Imgui Sample
This is very barebones sample to get a Imgui demo window running in vscode

Use a python install to run a config command like
```
fips set config sapp-d3d11-win64-vstudio-debug
```
or whatever target you want to compile

then run
```
fips build
```
which should generate all your libraries/dlls 

After that you should be able to use the debug button in vscode to run the cl.exe compiler