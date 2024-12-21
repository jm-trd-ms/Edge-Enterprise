---
title: "Microsoft Edge security for your business"
ms.author: archandr
author: seanongit
manager: likuba
ms.date: 07/18/2024
audience: ITPro
ms.topic: conceptual
ms.service: microsoft-edge
ms.localizationpriority: medium
ms.collection: M365-modern-desktop
description: "Microsoft Edge security for your business"
---

# Microsoft Edge security for your business

Microsoft Edge is built on top of the Chromium open source project—the same project that is core to Google Chrome—meaning it shares the same well-engineered and well-tested security architecture and design at its foundation. The Microsoft Edge security story doesn't stop there. It has powerful, built-in defenses against phishing and malware and natively supports hardware isolation on Windows—there's no additional software required to achieve this secure baseline. Furthermore, when paired with native support for Microsoft 365 security and compliance services, Microsoft Edge brings additional, powerful security capabilities and features that help protect against data loss for even more benefits. For more information, watch [Video: Microsoft Edge security, compatibility, and manageability](microsoft-edge-video-security-compatibility-manageability.md).

Let's get into the details, starting with **external threats** and then looking at **internal risks and information protection**.

## External threat protection

### Protection against phishing and malware

Built into Microsoft Edge, Microsoft Defender SmartScreen provides real-time reputation checks of sites and downloads as users work online, and is part of the [Microsoft Intelligent Security Graph](https://www.microsoft.com/microsoft-365/windows/intelligent-security), which draws signals and insights generated from Microsoft's large network of global assets, researchers, and partners. By running checks against dynamic, cloud-based lists of dangerous sites and downloads, Microsoft Edge helps to detect and block even ephemeral threats that quickly disappear.  

### The Microsoft Edge browser natively supports hardware isolation

The Microsoft Edge browser on Windows natively supports hardware isolation capabilities. As part of Windows Pro or Enterprise, Microsoft Defender Application Guard (Application Guard) runs untrusted sites in a kernel isolated from the local device and internal networks. The untrusted sites are run in a "container" so when an attack emerges, it's sandboxed from the rest of the corporate network. For more information, see [Microsoft Edge support for Application Guard](./microsoft-edge-security-windows-defender-application-guard.md).

For Chrome, an extension is available to use Windows hardware isolation—the MDAG extension. This extension launches Microsoft Edge in order to use Application Guard's kernel level isolation. Additionally, to achieve similar kernel level isolation for a Chrome-only solution, one needs third party isolation software.

> [!NOTE]
> Application Guard is available on Windows 10, 1809 and above. Application Guard isn't available on Windows 10 Home editions.

## Internal risks and information protection

### Native support for Microsoft 365 security without additional software

Aside from protecting against external threats, IT admins also must protect against internal risk. Protecting sensitive corporate data—robustly and at scale—is a top priority for IT administrators, particularly as workforces have decentralized. Microsoft Edge has native support for Microsoft Entra Conditional Access, Windows Information Protection, and the new Microsoft Endpoint Data Loss Prevention (DLP) without additional software required.

**Microsoft Edge natively supports Conditional Access**. [Microsoft Edge's support for conditional access](ms-edge-security-conditional-access.md) makes it easy for organizations to utilize identity signals as part of their access control decisions. [Conditional Access](/azure/active-directory/conditional-access/overview) is the tool used by Microsoft Entra ID to bring signals together, to make decisions, and enforce organizational policies. Conditional Access is at the heart of the new identity driven control plane. To get Conditional Access support on Chrome, an additional plug-in is required.

> [!NOTE]
> Microsoft Entra Conditional Access requires a Microsoft 365 E3 (or higher) or a Microsoft 365 Business Premium subscription.

**Microsoft Edge natively supports Windows Information Protection (WIP)**, which provides protection to corporate data to help prevent accidental leaks by users on Windows devices. [Microsoft Edge support for WIP](./microsoft-edge-security-windows-information-protection.md) can be configured to only allow IT mandated apps to access corporate data. It also provides leak controls—such as clipboard protection, encrypting files on download, and preventing file uploads to unauthorized network shares or cloud location — with a seamless user experience. WIP works on a perimeter-based configuration, where IT admins define the corporate boundary and all data inside that boundary is considered corporate.

> [!NOTE]
> Windows Information Protection (WIP) configuration requires licensing Microsoft Intune or Microsoft Endpoint Configuration Manager, or using a 3rd party mobile device management (MDM) solution, which might have additional licensing requirements.

**Microsoft Endpoint data loss prevention (Endpoint DLP) is supported natively in Microsoft Edge**. Endpoint DLP integrates with Microsoft Security Center and extends information protection to Microsoft Edge to help alert users to non-compliant activity and prevent data loss as users work online. It discovers and labels sensitive data inside the enterprise that matches admin-defined criteria, such as files containing credit card numbers or governmental IDs (for example, social security numbers), financial information, etc. Microsoft Information Protection policies can be deployed to Microsoft Endpoint DLP without additional reconfiguration, including sensitive content identifiers and policies that IT admins have already customized. This is seamless deployment of information protection for IT admins.

To learn more about Endpoint DLP prerequisites and how to set up data loss prevention, go to [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started?preserve-view=true&view=o365-worldwide).

> [!NOTE]
> Microsoft Endpoint data loss prevention requires a Microsoft 365 E5, a Microsoft 365 E5 Compliance, or a Microsoft 365 Business Premium subscription.

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
- [Video: Microsoft Edge security, compatibility, and manageability](microsoft-edge-video-security-compatibility-manageability.md)
