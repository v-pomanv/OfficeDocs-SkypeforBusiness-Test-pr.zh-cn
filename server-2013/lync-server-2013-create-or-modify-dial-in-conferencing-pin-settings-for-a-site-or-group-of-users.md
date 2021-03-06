﻿---
title: Lync Server 2013：创建或修改站点或用户组的电话拨入式会议 PIN 设置
TOCTitle: 创建或修改站点或用户组的电话拨入式会议 PIN 设置
ms:assetid: c29bab5c-2b93-48e0-ae0b-29564daaff9a
ms:mtpsurl: https://technet.microsoft.com/zh-cn/library/Gg412959(v=OCS.15)
ms:contentKeyID: 49314161
ms.date: 05/19/2016
mtps_version: v=OCS.15
ms.translationtype: HT
---

# 在 Lync Server 2013 中创建或修改站点或用户组的电话拨入式会议 PIN 设置

 

_**上一次修改主题：** 2012-10-18_

按照以下步骤创建或修改用户级别或站点级别电话拨入式会议的个人标识号 (PIN) 策略。有关如何更改全局 PIN 策略的详细信息，请参阅 [在 Lync Server 2013 中修改默认电话拨入式会议 PIN 设置](lync-server-2013-modify-the-default-dial-in-conferencing-pin-settings.md)。

## 创建用户或站点 PIN 策略

1.  使用 RTCUniversalServerAdmins 组成员（或具有同等用户权限）的用户帐户，或分配给 CsServerAdministrator 或 CsAdministrator 角色的用户帐户，登录到网络中部署了 Lync Server 2013 的任何计算机。

2.  打开浏览器窗口，然后输入管理 URL 以打开 Lync Server 控制面板。有关可以用于启动 Lync Server 控制面板的不同方法的详细信息，请参阅[打开 Lync Server 管理工具](lync-server-2013-open-lync-server-administrative-tools.md)。

3.  在左侧导航栏中，单击“会议”，然后单击“PIN 策略”。

4.  在“PIN 策略”页上，单击“新建”，然后执行下列操作之一：
    
      - 要创建用户级别的策略，请单击“用户策略”。在“新建 PIN 策略”的“名称”中，键入描述该策略的名称。
    
      - 要创建站点级别的策略，请单击“站点策略”。在“选择站点”搜索字段中，键入要为其创建策略的站点的全部或部分名称。在站点列表中，单击所需的站点，然后单击“确定”。

5.  在“说明”字段中，键入 PIN 策略的说明。

6.  在“最小 PIN 长度”字段中，键入或选择希望允许的最小 PIN 长度。默认的最小长度为 5 位数。

7.  为了能够指定锁定用户前允许的最大登录尝试次数，请选中“指定最大登录尝试数”复选框。如果未选择此选项，允许的最大尝试次数将根据 PIN 长度自动确定。默认情况下，最大尝试次数自动确定。

8.  如果选中了“指定最大登录尝试数”复选框，请在“最大登录尝试次数”中键入或选择希望允许的最大登录尝试次数。

9.  要使 PIN 过期，请选中“启用 PIN 有效期”复选框。如果未选择此选项，PIN 将永不过期。默认情况下，PIN 永不过期。

10. 如果选中了“启用 PIN 有效期”复选框，请在“PIN 有效期(天)”中键入或选择 PIN 保持有效的天数。

11. 在“PIN 历史记录计数”中，键入用户可以重复使用某个 PIN 之前，必须创建的 PIN 数目。默认情况下，用户可以重复使用其 PIN。

12. 要允许在 PIN 中使用数字的通用模式，如连续数字和重复数字集，请选中“允许通用模式”复选框。如果未选择此选项，则仅允许使用数字的复杂模式。默认情况下，仅允许使用数字的复杂模式。
    
    > [!IMPORTANT]
    > 我们建议您不要允许使用通用模式。


13. 单击“提交”。

## 更改用户或站点 PIN 策略

1.  使用 RTCUniversalServerAdmins 组成员（或具有同等用户权限）的用户帐户，或分配给 CsServerAdministrator 或 CsAdministrator 角色的用户帐户，登录到网络中部署了 Lync Server 2013 的任何计算机。

2.  打开浏览器窗口，然后输入管理 URL 以打开 Lync Server 控制面板。有关可以用于启动 Lync Server 控制面板的不同方法的详细信息，请参阅[打开 Lync Server 管理工具](lync-server-2013-open-lync-server-administrative-tools.md)。

3.  在左侧导航栏中，单击“会议”，然后单击“PIN 策略”。

4.  在“PIN 策略”页上，单击要更改的 PIN 策略，再单击“编辑”，然后单击“显示详细信息”。

5.  在“编辑 PIN 策略”中，修改任意策略设置（不能修改的策略名称除外）。

6.  单击“提交”。

