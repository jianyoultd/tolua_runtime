## tolua_runtime
**Build**<br>
pc: build_win32.sh build_win64.h  (mingw + luajit2.0.4) <br>
android: build_arm.sh build_x86.sh (mingw + luajit2.0.4) <br>
mac: build_osx.sh (xcode + luac5.1.5 luajit can't run in unity5) <br>
ios: build_ios.sh (xcode + luajit2.1 beta) <br>

NDK 版本:android-ndk-r10e 默认安装到 D:/android-ndk-r10e<br>
https://dl.google.com/android/repository/android-ndk-r10e-windows-x86_64.zip<br>
Msys2配置说明<br>
https://github.com/topameng/tolua_runtime/wiki<br>
配置好的Msys2下载<br>
https://pan.baidu.com/s/1c2JzvDQ<br>

## Libs
**cjson**<br>
https://github.com/mpx/lua-cjson<br>
**protoc-gen-lua**<br>
https://github.com/topameng/protoc-gen-lua<br>
**LuaSocket** <br>
https://github.com/diegonehab/luasocket<br>
**struct**<br>
http://www.inf.puc-rio.br/~roberto/struct/<br>
**lpeg**<br>
http://www.inf.puc-rio.br/~roberto/lpeg/lpeg.html



## iOS 版本添加拓展包并打包流程

- 将你需要添加的拓展包的 C 代码文件夹（如 cjson、sproto）放在项目要目录下

- 使用 mac 操作系统 ，进入 iOS 目录

- 确保已经装了 xcode 的情况下，双击 tolua.xcodeproj

- 选择 tolua 目录，并右键，选择 “Add Files to tolua”

![pic](./images/pic1.png)

- 选择你要添加的库

- 最后选择 Generic iOS Device ，并点击左边的 三角形运行即可

![pic](./images/pic2.png)

