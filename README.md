## obs-multi-rtmp OBS多路推流插件


### 安装
Windows版：
obs-plugins\64bit\obs-multi-rtmp.dll
data\obs-plugins\obs-multi-rtmp\locale
把obs-plugins和data这两个文件夹放到obs安装目录C:\Program Files\obs-studio

macOS版：
obs-multi-rtmp.plugin，这是编译好的插件，编译方式没问题的话这个插件是支持intel和M芯片的。
把obs-multi-rtmp.plugin插件放到$HOME/Library/Application Support/obs-studio/plugins目录下即可。


### 编译

按照OBS插件模板的编译方式编译即可。

[OBS插件模板工程](https://github.com/obsproject/obs-plugintemplate)

Windows版: 使用CMake构建出VS工程，然后用VS打开工程文件，编译即可。

macOS版：使用CMake生成XCode工程。
cmake --list-presets
cmake --preset macos
这个命令会自动下载编译插件需要的依赖库，并生成XCode工程，然后打开XCode工程进行编译即可。
