.. _intro/where-installers-should-put-plug-ins:

安装程序应将插件放在哪里？
################################################################################

在公共插件文件夹安装插件会使得 Premiere Pro 加载它们。

在 Windows 上，可以在以下注册表项中找到公共插件文件夹的详细路径：``HKLM\SOFTWARE\Adobe\After Effects\[版本]\CommonPluginInstallPath``

在 Mac 上，公共插件文件夹位于：``/Library/Application Support/Adobe/Common/Plug-ins/[版本]/MediaCore``

所有 CC 版本的版本号均锁定为 7.0，而早期版本均锁定为 CSx。例如：``/Library/Application Support/Adobe/Common/Plug-ins/7.0/MediaCore/``

不要使用 macOS 别名或 Windows 快捷方式。它们不会被 Premiere Pro 加载。

----

我必须将插件安装到公共插件文件夹吗？
================================================================================

有些时候，你希望你的插件只由 AE 加载，可能因为你的插件依赖于 Premiere Pro 不支持的功能。我们强烈建议你使用公共插件文件夹，但是特定于 AE 的插件文件夹也是可用的。

在 Windows 上，可以在以下注册表项中找到特定于 AE 的插件文件夹的详细路径：``\\HKEY_LOCAL_MACHINE\SOFTWARE\Adobe\After Effects\(版本)\PluginInstallPath``

在 macOS 上，特定于 AE 的插件文件夹位于：``/Applications/Adobe After Effects [版本]/Plug-ins/``

在启动时，AE 对插件目录进行深度为 10 级的递归遍历。macOS 的别名也会被遍历，但 Windows 快捷方式不会。不会扫描由括号终止或者开头有符号 ¬（macOS）或 ~（Windows）的目录。

虽然这样做可以让插件只由 AE 加载，但是 Premiere Pro 中仍然可以使用这些效果。用户可以在 AE 合成中应用效果，然后将合成动态链接进 Premiere Pro 的序列中。
