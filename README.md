SimpleUpdater.NET
=======================

## 简要说明 / Introduction

这是一个快速为已有的应用程序增加自动更新功能的组件，专为 .NET/WinForm 设计，虽然也可以通过命令行模式工作在其它语言中。
WPF将会在稍后支持。

This is a rapid application automatic updater component designed for .NET/WinForm and could be easily integrated into current applications. And it also can work for other applications via command line mode.
WPF support is on schedule.

```c#
FSLib.App.SimpleUpdater.Updater.CheckUpdateSimple("http://localhost/{0}", "update_c.xml");
```

### 特点 / Advantage

* 通过HTTP传输所有资料 / Using HTTP to perform update
* 全自动化，几乎不需要额外代码 / Fully automatically, almost no extra codes required
* 丰富的API接口事件，可定制化 / A large set events and customizable UI
* 提供打包工具，支持命令行打包 / Update package builder provided, supports build update packages via command line

## 基本集成步骤 / Basic steps to integrate

* Using package builder to build update packages
* Uploading update packages previously built to your server
* Add updater assembly ```SimpleUpdater.dll``` reference to your project (Recommand using Nuget package, add ```fishlee.net.simpleupdater``` package)
* Add update call to your ```Main()``` function


* 使用更新包构建工具创建更新包
* 上传生成的更新包到服务器目录中
* 在项目中添加 ```SimpleUpdater.dll``` 引用 （推荐使用Nuget包引用，搜索 ```fishlee.net.simpleupdater```）
* 在 ```Main()``` 函数中添加更新检查调用

## 发布和支持信息 / Release and Support

**软件发布主页 / Offical website** [http://www.fishlee.net/soft/simple_autoupdater/](http://www.fishlee.net/soft/simple_autoupdater/)

**使用建议 / Suggestion or Question** 可以在 [自动更新库知识社区] _(推荐)_ 或 [后花园论坛] 发帖询问

**更新日志 / Change Logs** [http://www.fishlee.net/soft/simple_autoupdater/#C-124](http://www.fishlee.net/soft/simple_autoupdater/#C-124)


[自动更新库知识社区]: http://ask.fishlee.net/category-19
[后花园论坛]: http://bbs.fishlee.net/