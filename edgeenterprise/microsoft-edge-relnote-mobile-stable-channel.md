---
title: "Microsoft Edge release notes for Mobile Stable Channel"
ms.author: charlielin
author: dan-wesley
manager: alexyuan
ms.date: 12/17/2024
audience: ITPro
ms.topic: conceptual
ms.service: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge release notes for Mobile Stable Channel"
---

# Release notes for Microsoft Edge Mobile Stable Channel

These release notes provide information about new features that are available to work or school accounts, and non-security updates that are included in the Microsoft Edge for Mobile Stable Channel.

To understand Microsoft Edge channels, see the [Overview of the Microsoft Edge channels](./microsoft-edge-channels.md).

All the Stable channel security updates are listed in [Release notes for Microsoft Edge Security Updates](./microsoft-edge-relnotes-security.md).

> [!NOTE]
> For the Stable Channel, updates roll out progressively over one or more days. To learn more, see [Progressive rollouts for Microsoft Edge updates](./microsoft-edge-update-progressive-rollout.md). There might be a delay before the new release is populated to the App Store (iOS) and Google Play (Android).

## Version 131.0.2903.107 (Android and iOS): December 17, 2024

Fixed various bugs and performance issues.

## Version 131.0.2903.101 (Android and iOS): December 13, 2024

Fixed various bugs and performance issues.

## Version 131.0.2903.87 (Android): December 9, 2024

Fixed various bugs and performance issues.


## Version 131.0.2903.77 (Android and iOS): December 2, 2024

Fixed various bugs and performance issues.

## Version 131.0.2903.68 (Android and iOS): November 25, 2024

Fixed various bugs and performance issues.

## Version 131.0.2903.54 (iOS): November 19, 2024

Fixed various bugs and performance issues, general updates, new policies, and enhancements.

### General updates

- [iOS] Upgrade Intune MAM SDK to version 19.7.2
- [iOS] Upgrade MAM Tunnel SDK to version 1.2.1
- [iOS] Upgrade MS OneAuth SDK version 4.0.2

### Bug fixes

- [iOS] Fix the issue with saving Word/Excel/PowerPoint files locally.
- [iOS] Fix unresponsive sign-in panel in "Send to device".
- [iOS] Fix the issue where the [IdleTimeout](/deployedge/microsoft-edge-mobile-policies#idletimeout) policy did not resume normal operation after the action was completed.
- [iOS] Fix Tooltip cannot auto-dismiss when VoiceOver is turned on.

### New Policies

- [iOS] Support to disable settings and feedback features via DisableFeature policy
(`com.microsoft.intune.mam.managedbrowser.disabledFeatures` in MAM and `EdgeDisabledFeatures` in MDM now supports configuring disable settings and feedback features on the NTP using the values "settings" and "feedback")
- [iOS] Support Microsoft Entra ID File advanced encryption by Intune auto file encryption capability. (Implement comprehensive encryption of sandbox files under Microsoft Entra ID accounts using Intune MAM SDK's File Transparent Encryption. File encryption is enabled when the `com.microsoft.intune.IntuneMAMOnly.AdvancedEncryption` policy is set to Enabled.)

### Enhancements

- [iOS] Improve the feature experience for the App Proxy policy by preventing it from not functioning correctly until the next cold start.
- [iOS] Improve the feature experience for switching profile.
- [iOS] General enhancements to [NewTabPageLayout](/deployedge/microsoft-edge-mobile-policies#edgenewtabpagelayout) policy (Policy auto correct NewTabPageLayout to custom if `NewTabPageLayout.Custom` has value).
- [iOS] Support sign-out action in [IdleTimeoutActions](/deployedge/microsoft-edge-mobile-policies#idletimeoutactions) policy.

## Version 131.0.2903.48 (Android): November 18, 2024

Fixed various bugs and performance issues, general updates, new policies, and enhancements.

### General updates

- [Android] Upgrade MS OneAuth SDK version 4.0.2

### New Policies

- [Android] Support to disable settings and feedback features via DisableFeature policy
(`com.microsoft.intune.mam.managedbrowser.disabledFeatures` in MAM and `EdgeDisabledFeatures` in MDM now supports configuring disable settings and feedback features on the NTP using the values "settings" and "feedback")

### Enhancements

- [Android] Enhancements the display size of brandLogo (Related policy `com.microsoft.intune.mam.managedbrowser.NewTabPage.BrandLogo`).
- [Android] Improve the sign-in experience for single device mode (Remove SDM needed restart on first startup).
- [Android] General enhancements to NewTabPageLayout policy (Policy auto correct NewTabPageLayout to custom if NewTabPageLayout.Custom has value).

## Version 130.0.2849.80 (Android and iOS): November 11, 2024

Fixed various bugs and performance issues.

## Version 130.0.2849.68 (Android and iOS): November 4, 2024

Fixed various bugs and performance issues.

## Version 130.0.2849.57 (Android and iOS): October 28, 2024

Fixed various bugs and performance issues.

## Version 130.0.2849.52 (iOS): October 23, 2024

Fixed various bugs and performance issues.

### General update

- [iOS] Upgrade Intune MAM SDK to version 19.7.2 which contains support for blocking of Apple Intelligence.

## Version 130.0.2849.46 (Android and iOS): October 20, 2024

Fixed various bugs and performance issues, general updates, new policies, and enhancements.

### General updates

- [iOS] Upgrade Intune MAM SDK to version 19.7.0
- [iOS] Upgrade MAM Tunnel SDK to version 1.1.12
- [iOS & Android] Enable wallpaper on NTP for Commercial user by default. A user can configure `com.microsoft.intune.mam.managedbrowser.NewTabPageLayout.Custom` to exclude the wallpaper.
- [iOS & Android] Enable weather widget on NTP for Commercial user by default. A user can add weather token to **DisableFeature** policy to disable it the widget.

### Bug fixes

- [iOS] Fix issue about single device mode force sign-in interrupted by external intent.
- [iOS] Fix **disableImportPasswords** policy not working as expected.

### New policies

- [iOS & Android] Support to disable weather widget on NTP via **DisableFeature** policy
(`com.microsoft.intune.mam.managedbrowser.disabledFeatures` in MAM) and **EdgeDisabledFeatures** in MDM, now supports disabling weather widget on NTP by using "weather" as value.

### Enhancements

- [iOS] Support removing specified account from sign in account list.
- [Android] Change default value of `recommendsCustomUi` to support passkey in Edge. Before these changes, the user can only use Google Password Manager and can't select Microsoft Authenticator to save passkey. After these changes, a user can select a third party passkey app, including Microsoft Authenticator.
- [Android] Improves the feature experience for App proxy.
- [iOS & Android] Improves the occurrence of re-sign in prompts on NTP.
- [iOS & Android] General enhancements to NTLMSSO policies to make it more useful.
- [iOS & Android] Enable Managed Browser revamp feature by default with silent mode as the managed browser. This change helps customers remediate from non-compliant cases, such as no device registration.

## Version 129.0.2792.92 (Android and iOS): October 15, 2024

Fixed various bugs and performance issues.

## Version 129.0.2792.84 (Android and iOS): October 9, 2024

Fixed various bugs and performance issues, enhancements.  

### Enhancements

- [Android and iOS] The page layout of the New Tab Page (NTP) defaults to Inspirational for Microsoft Entra ID accounts.

## Version 129.0.2792.65 (Android): September 27, 2024

Fixed various bugs and performance issues.

## Version 129.0.2792.58 (Android and iOS): September 24, 2024

Fixed various bugs and performance issues, general updates, bug fixes, enhancements, and new policies.

### General updates

- [iOS] Upgrade Intune MAM SDK to version 19.6.0
- [Android] Upgrade Intune MAM SDK to version 10.4.0
- [Android and iOS] Upgrade MS OneAuth SDK version 3.3.0 
- [Android and iOS] Remove native AAD Copilot support

### Bug fixes

- [iOS] Fix managed bookmarks dismiss under AAD account (without "XXX's Favorites" folder under favorites)
- [iOS] Fix downloaded files not properly moved in work profile
- [iOS] Fix a bug related to MAM Tunnel can't be disconnected automatically when change to personal account
- [iOS] Fix disableFeatures policy - InPrivate mode disablement bug & support policy auto change
(The problem is when set `com.microsoft.intune.mam.managedbrowser.disabledFeatures='inprivate'`, the InPrivate mode can still be accessed, and the corresponding toolbar button remains functional. Expects the policy to support dynamic switching without needing to restart Microsoft Edge. When the policy disables InPrivate mode, the application should automatically exit InPrivate mode and close all open InPrivate tabs)

### Enhancements

- [iOS] Improve the transition user experience for account switcher in iPad
- [iOS] Improve Web SSO for CMC (copilot.microsoft.com) sign in in MSA
- [Android and iOS] Improve the occurrence of re-sign-in prompts by disallow user interaction for proactive-auth
- [Android and iOS] Improve account verification by consider sync and news feed status
- [Android and iOS] General enhancements to NTLMSSO policies to make it more useful

### New Policies

- [Android and iOS] Support to disable Share and SendtoDevices via **DisableFeature** policy
(`com.microsoft.intune.mam.managedbrowser.disabledFeatures` in MAM and `EdgeDisabledFeatures` in MDM now support to config to disable Share and Sendtodevices in overflow menu by value share|sendtodevices)

<!-- Version 128.0.2739.82 (iOS): September 18, 2024 to Version 128.0.2739.42 (iOS): August 27, 2024 --->
<!-- Version 127.0.2651.111 (Android and iOS): August 20, 2024 to Version 127.0.2651.81 (iOS): July 31, 2024 --->
<!-- Version 126.2592.120 (iOS): July 24, 2024 to Version 126.0.2592.56 (Android and iOS): June 17, 2024 -->
<!-- Version 125.0.2535.96 (Android and iOS): June 11, 2024 to Version 125.0.2535.51 (Android): May 21, 2024 --->
<!-- Version 124.0.2478.105 (iOS): May 17, 2024 to Version 124.0.2478.50 (Android and iOS): April 22, 2024 -->
<!-- Version 123.0.2420.108 (iOS): April 19, 2024 to Version 123.0.2420.56 (iOS): March 25, 2024 -->
<!-- Version 122.0.2365.99 (Android and iOS): March 18, to 2024 Version 121.0.2277.84 (Android): January 29, 2024 -->
<!-- Version 120.0.2210.150: January 21, 2024 to Version 120.0.2210.59: December 12, 2023 -->
<!-- Version 119.0.2151.107: December 6, 2023 to Version 119.0.2151.46: November 7, 2023  -->
<!-- Version 118.0.2088.81: November 1, 2023 to Version 117.0.2045.53: October 6, 2023  -->
<!-- Version 117.0.2045.33: September 15, 2023 to Version 116.0.1938.64: August 30, 2023  -->
<!-- Version 116.0.1938.56: August 21, 2023, to Version 115.0.1901.183: July 22, 2023 -->
<!-- Version 114.0.1823.37: June 2, 2023 to Version 113.0.1774.50: May 18, 2023 -->
<!-- Version 113.1774.36: May 8, 2023 to Version 112.0.1722.36: April 7, 2023 -->
<!-- Version 111.0.1661.43: March 18, 2023 to Version 109.0.1518.70: January 26, 2023 -->
<!-- Version Version 109.0.1518.58: January 18, 2023 to Version 108.0.1462.45: December 8, 2022  -->
<!-- Version 108.0.1462.43: December 7, 2022 to Version 106.0.1370.47: October 17, 2022 -->
<!-- Version 105.0.1343.38: September 13, 2022 to Version 101.0.1210.32: April 29, 2022 -->

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
