---
title: "Hugo Test1"
date: 2018-09-21T11:22:20+08:00
draft: true
categories: "hugo"
tags: ["hugo"]
---

这是一个hugo 文档创建的例子

执行 hugo new /posts/hugo-test1.md 
1、对于APIInitialize、RemoteProcess或WebpageProcess等导出函数的参数类型由Integer改为QBInteger，可自适应Win32/Win64平台2、插件一定要Build为与主服务一致的平台类型（主服务是Win32的插件也Win32，否则都是Win64）3、通过传递地址来调用API函数时，务必注意Win32是4字节地址、Win64是8字节地址，使用指针、句柄时也一样4、Delphi 10.1 Update2等版本，在工程指定为Win64保存后，下次打开经常会变成Win32，务必小心使用，防止64位误操作变为32位DLL5、RemoteUnidac.dll数据库引擎模块默认用“Delphi 10.1 Update2+UniDAC 7.02”创建，如自己写的插件用到UniDAC引擎的API，也确保使用这样的版本来编译6、RemoteFiredac.dll数据库引擎模块默认也用“Delphi 10.1 Update2”创建，如自己写的插件用到FireDAC引擎的API，也确保使用这样的版本来编译7、如想用XE8、Tokyo等版本，则请对RemoteUnidac.dll、RemoteFiredac.dll重新用你的Delphi来Build一次、覆盖原来的，再继续写插件8、应尽量使用qbserviceapi.pas单元所提供的API接口类、弃用老的NodeServiceApi.pas里的API函数，因为前者已经处理好了32位/64位适应问题


