.. _intro/sdk-audience:

SDK 受众
################################################################################

想要做 After Effects 插件的开发，你必须是一个娴熟的 C/C++ 程序员。因为我们虽然会帮你解决与 After Effects API 相关的问题，但并不会帮助你去学习 IDE 和基本的编程技能。

你需要先熟悉 After Effects 和基本的 MG 术语。如果你对 AE 和相关术语还不甚了解，你可以通过这本书： `Adobe After Effects Classroom in a Book <http://www.adobepress.com/store/adobe-after-effects-cc-classroom-in-a-book-2017-release-9780134665320>`__ 或商城中的其他书籍去学习一下。它会帮助你学习如 alpha 通道，像素纵横比，隔行扫描，颜色空间等必须掌握的概念。

----

开发要求
================================================================================

After Effects 对系统的要求：https://helpx.adobe.com/after-effects/system-requirements.html

如果你需要旧版本的软件或 API 支持，请使用旧版 SDK（我们已经不再维护和提供旧版 SDK）。在当前版本发布六个月之后，我们将会停止支持和提供先前版本的 SDK。

我们为 macOS 10.11 上的 Xcode 7.3，和 Windows 7 64 或 Windows 10 上的 Microsoft Visual Studio 2015 创建了 SDK 样板。你可能发现了，我们对 IDE 的要求很严格。换成新的编译器确实不是个简单的事，但我们也确实不会继续对更老的开发环境提供帮助。

若要使用 Visual Studio，你可能需要修改安装设置以下载 64 位编译器组件。你可能会使用 Visual Studio Express，但你仍需下载 64 位编译器组件。请参考：http://msdn.microsoft.com/en-us/library/9yb4317s.aspx

若要用更新版本的 Xcode 或 macOS 编译，你只需要在 Build Settings（构建设置）中更新一下当前版本的 SDK 即可。 
