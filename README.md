# vscode源码编译

## 配置编译环境

1.Xcode和命令行工具，它们将安装gcc以及包含的相关工具链make
运行xcode-select --install以安装命令行工具

## 安装依赖包

```
cd vscode
yarn

yarn watch 本地调试编译
./scripts/code.sh  启动vscode

```

## 调试源码

1.安装Debugger for Chrome扩展程序
2.打开命令面板 输入Toggle Developer Tools

## 启动web版vscode

```
yarn watch web
yarn web

```

# 屏蔽从插件市场下载插件，国内或公司网络限制很难下载
task.define('bundle-marketplace-extensions-build', () => ext.packageMarketplaceExtensionsStream(false).pipe(gulp.dest('.build')))

# pushd %~dp0\..
"用PUSHD获得bat文件执行的路径"

# VsCode源码分析之布局
1.titlebar D:\git\vscode\hpaas-studio\src\vs\workbench\browser\parts\titlebar
2.activitybar
3.sidebar
4.statusbar
5.welcome
6.
