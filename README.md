# C++ Project Starter Template

## C++ 项目入门模板
这是一个小型的快速启动项目模板，适用于使用Core/App 项目架构的 C++ 项目。其中包含两个项目 - 一个名为Core，一个名为App。Premake用于生成项目文件。

Core 构建为静态库，旨在包含用于多个应用程序的通用代码。App 构建为可执行文件并链接 Core 静态库，并提供 Core 代码的包含路径。

该Scripts/目录包含适用于 Windows 和 Linux 的构建脚本，该Vendor/目录包含 Premake 二进制文件（当前版本5.0-beta2）。

## 入门
克隆此存储库或使用 GitHub 上的“使用此模板”按钮，基于此模板快速设置您自己的存储库
App/和Core/是两个项目 - 您可以编辑这些文件夹的名称及其内容以适合
包含的三个 Premake 构建文件是Build.lua、Core/Build-Core.lua和App/Build-App.lua- 您可以编辑这些文件来自定义构建配置、编辑项目和工作区/解决方案的名称等。
打开Scripts/目录并运行相应的Setup脚本以生成项目文件。您可以编辑设置脚本以更改生成的项目类型 - 开箱即用，它们设置为 Windows 的 Visual Studio 2022 和 Linux 的 gmake2。
请注意，目前没有提供 macOS 安装脚本；您可以复制 Linux 脚本并进行相应调整。

## 包括
一些示例代码（在App/Source和中Core/Source）提供起点和测试
简单.gitignore忽略项目文件和二进制文件
适用于 Win/Mac/Linux 的预制作二进制文件 ( v5.0-beta2)

## 执照
取消此存储库的许可（查看UNLICENSE.txt更多详细信息）
Premake 遵循 BSD 3-Clause 许可（有关详细信息，请参阅随附的 LICENSE.txt 文件）
