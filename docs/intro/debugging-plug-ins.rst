.. _intro/debugging-plug-ins:

调试插件
################################################################################

学习 After Effects 和插件之间交互的最好的方法就是在调试程序中运行这些示例。花一些时间在你的编译器的调试程序和一个与你的插件紧密关联的实例中，你将会受益匪浅。

当你如之前提到过的一样，将插件直接构建如插件文件夹中之后，下面是让 After Effects 运行在调试期间的方法：

在 Windows 系统中：

1) 在 Visual Studio 的 solution 中，于 Solution Explorer 面板选择你想要调试的 project
2) 右键点击并将其设置为 StartUp Project
3) 再次右键点击你选择的 project 并选择 Properties
4) 在 Configuration Properties > Debugging > Command 中，提供运行插件的应用程序的可执行文件的路径（这里的应用程序应该是 After Effects 或 Premiere Pro）
5) 现在你可以点击 Play 按钮， 或者你可以启动应用程序并稍后选择 Debug > Attach to Process...

在 macOS 系统中:

1) 在 Xcode 中，于 Project Navigator 选择你想调试的 xcodeproj
2) 选择 Project > Scheme > Edit Scheme...
3) 在 Run 下的 Info 标签中，选择用来运行插件的应用程序（这里为 After Effects 或 Premiere Pro）
4) 现在，你可以点击 Play 按钮来构建和运行当前的方案，或者启动应用程序并稍后选择 Debug > Attach to Process

----

.. _intro/debugging-plug-ins.deleting-preferences:

清理偏好
================================================================================

在开发学习插件的过程中，你的插件可能会给 After Effects 传输一些设置信息，这些信息会被储存在偏好文件之中。

你可以在 After Effects 启动时通过  Ctrl-Alt-Shift / Cmd-Opt-Shift 快捷键来清除偏好设置并以初始状态重新启动程序。

在 windows 系统中，偏好文件被储存在以下路径中：``[user folder]\AppData\Roaming\Adobe\After Effects\[version]\Adobe After Effects [version]-x64 Prefs.txt``

在 macOS 系统中，则在以下路径：``~/Library/Preferences/Adobe/After Effects/[version]/Adobe After Effects [version]-x64 Prefs``
