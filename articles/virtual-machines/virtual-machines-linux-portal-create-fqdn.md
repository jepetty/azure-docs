---
title: Create FQDN for a Linux VM in the Azure portal | Microsoft Docs
description: Learn how to create a Fully Qualified Domain Name, or FQDN, for a Resource Manager based virtual machine in the Azure portal.
services: virtual-machines-linux
documentationcenter: ''
author: iainfoulds
manager: timlt
editor: tysonn
tags: azure-resource-manager

ms.assetid: 2cd6c249-a737-4a0a-b5ba-e1c09e551b30
ms.service: virtual-machines-linux
ms.devlang: na
ms.topic: article
ms.tgt_pltfrm: vm-linux
ms.workload: infrastructure-services
ms.date: 03/14/2017
ms.author: iainfou
ms.custom: H1Hack27Feb2017

---
# Create a Fully Qualified Domain Name in the Azure portal for a Linux VM

When you create a virtual machine (VM) in the [Azure portal](https://portal.azure.com) using the Resource Manager deployment model, a public IP resource for the virtual machine is automatically created. You use this IP address to remotely access the VM. Although the portal does not create a [fully qualified domain name](https://en.wikipedia.org/wiki/Fully_qualified_domain_name), or FQDN, by default, you can add one once the VM is created. This article demonstrates the steps to create a DNS name or FQDN.

[!INCLUDE [virtual-machines-common-portal-create-fqdn](../../includes/virtual-machines-common-portal-create-fqdn.md)]

You can now connect remotely to the VM using this DNS name such as with `ssh ops@mydns.westus.cloudapp.azure.com`.

## Next steps
Now that your VM has a public IP and DNS name, you can deploy common application frameworks or services such as nginx, MongoDB, Docker, etc.

You can also read more about [using Resource Manager](../azure-resource-manager/resource-group-overview.md) for tips on building your Azure deployments.

