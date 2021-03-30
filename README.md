[中文说明](./README_CN.md)

# Special Statement

This project is modified from [Actions-OpenWrt](https://github.com/P3TERX/Actions-OpenWrt)，thank you very much for the work of P3TERX 🙏 。

## Build-OpenWrt-R7800

Build OpenWrt using GitHub Actions For Nighthawk X4S R7800

## Include Plug-in List

- SSR-PLUS （socket clietn）
- OpenClash （Clash client）
- SFE （Turbo ACC）

## Usage

- Click the [Use this template](https://github.com/brick713/Build-OpenWrt-R7800) button to create a new repository.
- Generate `.config` files using [Lean's OpenWrt](https://github.com/coolsnowwolf/lede) source code. ( You can change it through environment variables in the workflow file. )
- Push `.config` file to the GitHub repository, and click the `star` button, the build starts automatically.Progress can be viewed on the Actions page.
- When the build is complete, click the `Artifacts` button in the upper right corner of the Actions page to download the binaries.
- Compilation will be executed at 18:00 every Friday，You can modify the `cron` parameter in the `config` file to customize.

## Tips

It may take a long time to create a `.config` file and build the OpenWrt firmware. You can use my profile `.config` Compile your own firmware after modifying it according to your needs

Add some meta info of your built firmware (such as firmware architecture and installed packages) to your repository introduction, this will save others' time.

