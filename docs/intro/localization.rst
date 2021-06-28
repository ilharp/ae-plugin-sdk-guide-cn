.. _intro/localization:

本地化
################################################################################

从CC版本开始，PF应用套件(:ref:`effect-details/useful-utility-functions`)会添加``PF_AppGetLanguage()``用来查询当前使用的语言，这样一来，插件便可以使用正确语言的字串。

在向AE发送字串时，API的一部分可以采用Unicode。在特殊情况，比如在``PF_Cmd_PARAM_SETUP``中指定效果参数名称时，你需要将名称通过char类型的字串进行传递。对于这些非Unicode的字串，AE会将他们认作是针对应用程序当下区域设置生成的多字节编码。如果想创建这样的字串，在Windos上你可以使用``WideCharToMultiByte()``函数，并将首个参数设置为``CP_OEMCP``。在macOS上，则可以使用``GetApplicationTextEncoding()``返回的编码。

在AE上测试并切换不同的语言不需要重新安装操作系统，但要求重新安装AE。

针对Win操作系统，保证系统地区与想修改的语言保持一致(control panel 控制面板> region and language 地区和语言> administrative tab 管理标签> change system locale 更改系统地区)，更改完毕后重启计算机并以正确的语言下载AE。

对于Mac操作系统，将想修改为的语言在语言偏好列表里设置为首选语言，更改完毕后以正确的语言下载AE。
