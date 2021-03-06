﻿---
title: 'Lync Server 2013: Running synthetic transactions'
TOCTitle: Running synthetic transactions
ms:assetid: 2b56c7bd-8956-4fa1-8232-1876b959b258
ms:mtpsurl: https://technet.microsoft.com/zh-cn/library/Dn720911(v=OCS.15)
ms:contentKeyID: 62246682
ms.date: 05/19/2016
mtps_version: v=OCS.15
ms.translationtype: HT
---

# Running synthetic transactions in Lync Server 2013

 

_**上一次修改主题：** 2014-08-18_

Synthetic transactions are typically conducted in two ways. You can use the CsHealthMonitoringConfiguration cmdlets to set up test users for each of their Registrar pools. These test users are a pair of users who were preconfigured for use with synthetic transactions. (Typically these are test accounts and not accounts that belong to actual users.) With test users configured for a pool, you can run a synthetic transaction against that pool without having to specify the identities of (and supply the credentials for) the user accounts involved in the test.

Or, you can run a synthetic transaction by using actual user accounts. For example, if two users cannot exchange instant messages, you could run a synthetic transaction using those two user accounts (instead of a pair of test accounts), and then try to diagnose and resolve the issue. If you decide to conduct a synthetic transaction using actual user accounts, you must supply the logon names and passwords for each user.

## 另请参阅

#### 概念

[配置观察程序节点测试用户和配置设置](lync-server-2013-configuring-watcher-node-test-users-and-configuration-settings.md)  
[综合事务的特殊设置说明](lync-server-2013-special-setup-instructions-for-synthetic-transactions.md)

