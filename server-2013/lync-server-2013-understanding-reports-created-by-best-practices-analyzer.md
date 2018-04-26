﻿---
title: 了解由最佳做法分析器创建的报告
TOCTitle: 了解由最佳做法分析器创建的报告
ms:assetid: 1386dd6c-7f3e-4da9-905b-cef1468bf14a
ms:mtpsurl: https://technet.microsoft.com/zh-cn/library/Gg591344(v=OCS.15)
ms:contentKeyID: 49312077
ms.date: 05/19/2016
mtps_version: v=OCS.15
ms.translationtype: HT
---

# 了解由最佳做法分析器创建的报告

 

_**上一次修改主题：** 2012-10-10_

最佳做法分析器提供多种类型的报告，旨在促进问题的分析和解决。最佳做法分析器可标识问题，如错误、警告和其他信息。

## 报告

通过查看以下每个报告可以访问扫描结果：

  - **列表报告**   列表报告按特定条件来组织。可以按类、严重性或问题来排列结果。例如，如果按类组织结果，则与控制器相关的问题将包括在报告的“控制器”部分下。可以查看所有问题，或只查看信息性项目。可在列表报告中搜索特定项，如内存。还可以打印报告或导出报告。

  - **目录树报告**   目录树报告按用于运行扫描的规则和在运行扫描时指定的其他选项来组织。例如，与“测试拓扑”规则相关的问题包括在报告的“测试拓扑”部分下。可以查看所有问题的详细信息，或只查看问题的摘要。可在目录树报告中搜索特定项，如内存。还可以打印报告或导出报告。

  - **其他报告**   其他报告中的项包括扫描中包含的任务的运行时日志。可搜索其他报告中的项目以查找特定项（如内存）。还可以打印报告或导出报告。

## 问题

最佳做法分析器生成的报告指示在扫描环境期间标识的特定问题，包括以下类型的问题：

  - **错误**   需要您在环境中进行更改的关键问题。例如，如果未安装 Lync Server 2013 核心组件，则会记录错误。
    
    分类为错误的问题在报告中用红色的 X 符号来标识。错误显示在“列表报告”视图的“所有问题”选项卡以及“目录树报告”视图的“详细视图”选项卡和“摘要视图”选项卡上。如果不想在报告中查看特定错误，可以指定不在报告中为该错误的单个实例或所有实例显示该错误。然后，除非您更改设置并指定在报告中显示该错误，否则该错误将只在“其他报告”视图的“已隐藏项”选项卡中显示。

  - **警告**   与最佳实践的实现不一致的问题。这可能表示环境中需要或不需要更改。该问题可能是无需更改的特定设置的已知问题。例如，未在服务器中启动的服务记录为警告。
    
    分类为警告的问题在报告中用三角形的黄色警告符号来标识。警告显示在“列表报告”视图的“所有问题”选项卡以及“目录树报告”视图的“详细视图”选项卡和“摘要视图”选项卡上。如果不想在报告中查看特定错误，可以指定不在报告中为该错误的单个实例或所有实例显示该错误。然后，除非您更改设置并指定在报告中显示警告，否则该警告将只在“其他报告”视图的“已隐藏项”选项卡中显示。

  - **信息**   包括未分类为错误或警告的所有问题。例如，Active Directory 域服务 中的 Lync Server 2013 Standard Edition 服务器对象数被分类为信息问题。
    
    信息问题显示在“列表报告”视图的“所有问题”选项卡和“目录树报告”视图的“详细视图”选项卡上。

Lync Server 2013 最佳做法分析器不对环境进行更改，以解决问题。扫描仅检测潜在问题，并提供包含有关如何解决每个问题的信息的报告。

如果单击某个问题，则会显示特定问题的解释和一些选项。然后，您可以执行以下任何操作：

  - 查找有关问题的更详细信息以及如何解决问题。

  - 停止在报告中显示问题：
    
      - 停止为选定实例显示问题。
    
      - 停止为该问题的所有实例显示问题。
    
    若要查看已在报告中停止显示的问题，请转到“其他报告”视图的“已隐藏项”选项卡。在此，可以指定在报告中重新开始显示问题。

有关解决特定问题的详细信息，请参阅[分析和解决由最佳做法分析器标识的问题](lync-server-2013-analyzing-and-resolving-issues-identified-by-best-practices-analyzer.md)。
