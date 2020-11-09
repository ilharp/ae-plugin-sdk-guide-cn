After Effects 插件 SDK 指南（中文版）
################################################################################

这个项目存放了 RST 格式的 After Effects 插件 SDK 指南文档，并且部署在 http://ae-plugin-sdk-cn.vbox.moe

----

贡献
################################################################################

我们欢迎贡献。查看下面的内容以了解参与贡献的流程。

在参与翻译之前，请先前往 `翻译计划概要 <https://github.com/Afanyiyu/ae-plugin-sdk-guide-cn/issues/1>`_ 了解目前翻译的主要方向和进度，然后在下方回复以申领任务。这样可以避免任务冲突或重复的提交。

推荐通过发起带有 ``WIP`` 字样的提交请求来确定自己的任务。发起了 PR 之后，你就可以在 `项目 <https://github.com/Afanyiyu/ae-plugin-sdk-guide-cn/projects/1>`_ 中进行翻译进度的跟踪了。推荐使用 ``author-name/section-name`` 作为源分支名称。

其他一些错别字的修改或小的修改可以直接开启 PR。

进行修改时，请务必保证自己的修改是最小的。不要更改文档的结构和其他与文本无关的内容。

RST 格式指南可以参考下方的引用，也可以参考 `reStructuredText 简介 <https://zh-sphinx-doc.readthedocs.io/en/latest/rest.html>`_。

----

Internal References
********************************************************************************

Anchors should be defined at each page setting relative to the root folder; the anchor for the "Application" page within the JS Object Reference should be::

  .. _jsobjref/Application

And the anchor for a child item (property, method or example)::

  .. _jsobjref/Application.open

Then, to link to these items from other pages, we use::

  :ref:`jsobjref/Application`

or::

  :ref:`jsobjref/Application.open`

If you want different text than the title the anchor points to::

  :ref:`Check this out! <jsobjref/Application.open>`

----

External Links
********************************************************************************

These should follow the following structure::

  `Link Text <http://www.aenhancers.com>`__

----

Tables
********************************************************************************

Function parameter tables should have following order::

  +---------------+------+-----------------------------+
  |   Parameter   | Type |         Description         |
  +===============+======+=============================+
  | ``parameter`` | Type | What does the parameter do? |
  +---------------+------+-----------------------------+

Use `Table Formatter <https://marketplace.visualstudio.com/items?itemName=shuworks.vscode-table-formatter>`_ for VSCode for easier table formating.

----

Admonitions Usage
********************************************************************************

Currently, the following `admonitions <http://docutils.sourceforge.net/docs/ref/rst/directives.html#admonitions>`_ are in use in this project.

Try to keep one piece of data per note, for easier parsing.

::

  .. note::
    Notes detail version added, and/or relevant pieces of information.

  .. tip::
    Tips supply helpful suggestions on usage or behaviours.

  .. warning::
    Warnings convey negative behaviours, or when something won't work the way you'd expect.

----

本地构建 HTML
################################################################################

You may want to build the HTML locally before pushing, in order to ensure that the result is what you'd expect. These files aren't included in the git repo, nor are they used online; this is solely to create a local, offline version of the online docs.

- Install ``Python 2.7``
- Install ``pip``
- Navigate to the project directory and use the command ``pip install -r requirements.txt``
- Build the docs using ``make html``

----

许可
################################################################################

本项目只限学习研究使用。一切内容之权利均归 Adobe Systems Incorporated 所有。
