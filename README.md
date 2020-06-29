FlatUI
======

FlatUI是一个应用于python3.x的图形界面库。

FlatUI的概念来源于HTML的CSS理念，也参考了tkinter的ttk库。库中的窗体对象（Component）定义了数据和控制接口，将显示属性分离，可由单独的style文件来定义，起到代码复用和风格统一的功能。


窗体对象（Component）
------------------

FlatUI中的每个窗体对象都由Component继承来。一个Comonent包含如下属性：

* 数据对象（Data）
* 控制接口（Listener）
* 外观属性（Style)
* 布局属性（Layout）

其中的外观属性和布局属性都可以由风格系统（style system）参与更新。

FlatUI中支持的窗体类列表：

* [ ] View
* [ ] Label
* [ ] Image
* [ ] Button
* [ ] Checkbox
* [ ] Radiobox
* [ ] Combobox
* [ ] List
* [ ] Table
* [ ] Tree
* [ ] Scrollbar
* [ ] Progressbar
* [ ] Indicator
* [ ] ScrollView
* [ ] TabView
* [ ] TextField
* [ ] TextArea


风格系统（Style System）
---------------------

每个窗体对象都有一些通用的外观属性，也会有自己独有的外观属性。这些属性可以由Component自己定义，也可以在风格系统中定义。每个属性的定义优先级为：

1. 窗体对象的显式定义
1. 风格系统中的选中定义
1. 窗体类中的缺省定义

外观属性在窗体属性发生改变的时候，会根据上述优先级进行一次计算，得到窗体对象的最终属性值，用于控制后端实现。


后端（Backend）
-------------

FlatUI可以接入不同的后端，计划的backend有：

* [ ] Tkinter
* [ ] MacOS Cocoa
* [ ] Win32 API
* [ ] PyQT5


开源协议（License）
----------------

GPLv3


