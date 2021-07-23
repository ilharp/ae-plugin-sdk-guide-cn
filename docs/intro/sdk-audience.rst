.. _intro/sdk-audience:

SDK 受众
################################################################################

想要做 After Effects 插件的开发，你必须是一个娴熟的 C/C++ 程序员。因为我们虽然会帮你解决与 After Effect API 相关的问题，但并不会帮助你去学习 IDE 和基本的编程技能。

这个 SDK 手册将认为你是一个熟悉 After Effects 和基本动态图像术语的用户。如果你对 AE 和相关术语还不甚了解，你可以通过一本书： `Adobe After Effects Classroom in a Book <http://www.adobepress.com/store/adobe-after-effects-cc-classroom-in-a-book-2017-release-9780134665320>` 或商城中的其他书籍去学习一下。

他会帮助你学习如 alpha 通道，像素纵横比，隔行扫描，颜色空间等必须掌握的概念。

----

开发要求
================================================================================

After Effects 对系统的要求如下: https://helpx.adobe.com/after-effects/system-requirements.html

如果你需要旧版本的软件或 API 支持，请使用旧的 SDK （我们不再维护和提供的那种）。在当前版本发布六个月之后，我们将会停止提供与支持先前版本的 SDK。

我们为 macOS 10.11 上的 Xcode 7.3，和 Windows 7 64 或 Windows 10 上的 Microsoft Visual Studio 2015 创建了 SDK 样板。是的，你可能发现了，我们对 IDE 的要求很严格。换成新的编译器不是个简单的事，我们也不会继续针对更老的开发环境提供帮助。

想要使用 Visual Studio，你可能会需要调整一些安装设置，去下载一些用来编译 64 比特插件的组件。你可能会使用 Visual Studio Express，但你仍需下载一些额外的组件用来编译 64 比特的插件，正如以下所描述的： http://msdn.microsoft.com/en-us/library/9yb4317s.aspx

想要用更新版本的 Xcode 或 macOS 去编译的时候，基本上你只需要在 Build Settings （构建设置）中更新一下当前版本的 SDK 就可以了。 
