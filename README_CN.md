# 特别说明

本项目修改自[Actions-OpenWrt](https://github.com/P3TERX/Actions-OpenWrt)，非常感谢🙏 P3TERX 的工作。

## 项目简介

本项目通过 Github Actions 为网件的 R7800（Nighthawk X4S R7800） 编译基于 Lean 开发的 OpenWrt 固件。

## 插件列表

该项目基于个人喜好，删除了大部分不需要使用的插件，编译过程中主要添加了以下插件，如果你有其他需求请自行修改配置文件添加插件。

- SSR-PLUS （socket clietn）
- OpenClash （Clash client）
- SFE （Turbo ACC网络加速）

## 使用方法

- Fork 该项目 [Use this template](https://github.com/brick713/Build-OpenWrt-R7800) 创建一个属于你自己对全新分支。
- 你可以默认使用我的 `.config` 配置通过使用 [Lean's OpenWrt](https://github.com/coolsnowwolf/lede) 的源码进行编译( 您可以自行修改 workflows 中的环境变量来更改相关配置，这里不做详细展开)。
- 每次更新`.config`文件后，并 Push 到 GitHub 仓库中，`star` 项目后构建就会自动开始，进度可以在`Actions`页面上查看，但这里不推荐频繁但构建。
- 构建完成后，在 `Actions` 页面进入你最新的一次构建，然后在`Artifacts`下方下载二进制文件，根据你自身情况找到对应的固件文件类型，按需刷入。
- 编译会在每周五的 18:00 自动进行编译，你可以修改`config`文件中的`cron`参数自行修改。


## 建议

创建`.config`文件并构建OpenWrt固件可能需要很长时间。您可以使用我的配置文件`.config`,根据需要修改配置文件后,编译自己的固件。

如果你修改了相关配置，建议将您所构建固件的一些元信息（例如固件体系结构和已安装的软件包）添加到存储库简介中，这将节省其他人的时间。

祝你使用愉快。