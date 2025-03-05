---
title: "Microsoft Edge release notes for Stable Channel"
ms.author: archandr
author: vmliramichael
manager: likuba
ms.date: 02/27/2025
audience: ITPro
ms.topic: conceptual
ms.service: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge release note for Stable Channel"
---

# Release notes for Microsoft Edge Stable Channel

These release notes provide information about new features and nonsecurity updates that are included in the Microsoft Edge Stable Channel.

- All the security updates are listed in [Release notes for Microsoft Edge Security Updates](./microsoft-edge-relnotes-security.md).
- Archived release notes for Microsoft Edge Stable Channel are located in [Archived release notes for Microsoft Edge Stable Channel](./microsoft-edge-relnote-archive-stable-channel.md).

 To understand Microsoft Edge channels, see the [Overview of the Microsoft Edge channels](./microsoft-edge-channels.md).

> [!NOTE]
> For the Stable Channel, updates roll out progressively over one or more days. To learn more, see [Progressive rollouts for Microsoft Edge updates](./microsoft-edge-update-progressive-rollout.md).
>
> Microsoft Edge Web Platform constantly evolves to improve user experience, security, and privacy. To learn more, see [Site compatibility-impacting changes coming to Microsoft Edge](/microsoft-edge/web-platform/site-impacting-changes).

## Version 132.0.2957.178: February 27, 2025

Fixed various bugs and performance issues for Extended Stable Channel.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#february-27-2025).

## Version 133.0.3065.92: February 27, 2025

Fixed various bugs and performance issues for Stable Channel.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#february-27-2025).

## Version 133.0.3065.82: February 21, 2025

Fixed various bugs and performance issues for Stable Channel.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#february-21-2025).

## Version 132.0.2957.171: February 20, 2025

Fixed various bugs and performance issues for Extended Stable Channel.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#february-20-2025).

## Version 133.0.3065.69: February 14, 2025

Fixed various bugs and performance issues.

### Fixes

- Fixed an issue which caused excessive traffic to the MIP service and resulted in the temporary blocking of sync functionality and the inability to open AIP-protected PDF files in Edge.  Note: For some users it still might be necessary to "sign out (keeping locally saved data)"and then "sign-in" again for sync functionality to resume.  

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#february-14-2025).

## Version 132.0.2957.164: February 13, 2025

Fixed various bugs and performance issues for Extended Stable Channel.

## Version 133.0.3065.59: February 10, 2025

Fixed various bugs and performance issues.

## Version 132.0.2957.158: February 10, 2025

Fixed various bugs and performance issues for Extended Stable Channel.

## Version 133.0.3065.51: February 6, 2025

Fixed various bugs and performance issues, Dev channel updates, feature updates, policy updates, and web platform release notes.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#february-06-2025).

### Dev Channel updates

The following Dev channel updates preceded this Stable channel release. The following Dev notes provide detailed information about the changes in each release.

- [Dev Channel update to 133.0.2992.0 is live. | Microsoft Community Hub](https://techcommunity.microsoft.com/discussions/edgeinsiderannouncements/dev-channel-update-to-133-0-2992-0-is-live-/4354854)
- [Dev Channel update to 133.0.3000.0 is live. | Microsoft Community Hub](https://techcommunity.microsoft.com/discussions/edgeinsiderannouncements/dev-channel-update-to-133-0-3000-0-is-live-/4357092)
- [Dev Channel update to 133.0.3014.0 is live. | Microsoft Community Hub](https://techcommunity.microsoft.com/discussions/edgeinsiderannouncements/dev-channel-update-to-133-0-3014-0-is-live-/4359765)
- [Dev Channel update to 133.0.3054.1 is live. | Microsoft Community Hub](https://techcommunity.microsoft.com/discussions/edgeinsiderannouncements/dev-channel-update-to-133-0-3054-1-is-live-/4364687)
- [Dev Channel update to 133.0.3065.7 is live. | Microsoft Community Hub](https://techcommunity.microsoft.com/discussions/edgeinsiderannouncements/dev-channel-update-to-133-0-3065-7-is-live-/4367429)

### Fixes

- Fixed an issue which prevented users from selecting 'Report this file as safe' when downloading a file.

### Feature updates

- **Extending support for viewing MIP Protected PDF Files to different sovereignties (including GCCH).** Sovereign cloud customers (including GCCH) are able to open MIP protected PDF content in Microsoft Edge. This change is available in the Microsoft Edge built-in PDF reader powered by Adobe Acrobat and the legacy Microsoft Edge PDF engine.

- **Non-special scheme URL handling.** Nonspecial scheme URL handling is updated to become compliant with the URL Standard (https://url.spec.whatwg.org/). This change has site compatibility impacts which might require changes to your web sites. For more information and web developer guidance, see http://bit.ly/url-non-special.
 
- **Deprecate `textprediction` attribute.** Removes support for the `textprediction` HTML attribute, which is a nonstandard attribute that's used to enable or disable the browser-based Text Prediction feature for long-form text inputs. Instead, use the standardized `writingsuggestions` attribute, which functions similarly to `textprediction`, but also applies to other writing-assistance features that browsers may provide. Sites that explicitly set `textprediction` to `true` or `false` can instead set `writingsuggestions` to the same value. For more information, see [Writing suggestions](https://html.spec.whatwg.org/multipage/interaction.html#writing-suggestions) in the HTML specification.

- **Scareware blocker.** Scareware blocker in Microsoft Edge is your AI powered shield designed to protect you and your users from scareware attacks. Once enabled, scareware blocker uses machine learning (ML) to identify and block these scams, keeping you safe as you browse the web. For more information, [see Stand up to scareware with scareware blocker](https://blogs.windows.com/msedgedev/2025/01/27/stand-up-to-scareware-with-scareware-blocker/). Note: This experience is in preview and users can opt in via Microsoft Edge Settings, under `edge://settings/privacy`, Scareware is located under “Security”.
 
- **Remove policy used for legacy same site behavior.** In Microsoft Edge version 80, we introduced the [LegacySameSiteCookieBehaviorEnabledForDomainList](/deployedge/microsoft-edge-policies#legacysamesitecookiebehaviorenabledfordomainlist) policy to revert the SameSite behavior of cookies to legacy behavior on the specified domains. The [LegacySameSiteCookieBehaviorEnabledForDomainList](/deployedge/microsoft-edge-policies#legacysamesitecookiebehaviorenabledfordomainlist) policy is obsolete in Microsoft Edge version 133.
 
- **Updated Downloads UI to Improve Performance.** The Downloads UI is rewritten to improve performance. Customer-facing functionality and UX from previous releases remain the same.

- **Shopping Product Tracking.** Track product prices easily with a new experience in the Edge Address Bar that appears on the product detail page.  Users can track prices quickly and will be notified when there is a price drop on that product and save more.  Administrators can control the availability of Shopping in Edge using the [EdgeShoppingAssistantEnabled](/deployedge/microsoft-edge-policies#edgeshoppingassistantenabled) policy.

### Policy updates

#### New policies

- [CACertificateManagementAllowed](/deployedge/microsoft-edge-policies#cacertificatemanagementallowed)- Allow users to manage installed CA certificates
- [CA Certificates](/deployedge/microsoft-edge-policies#cacertificates) - TLS server certificates that should be trusted by Microsoft Edge
- [CACertificatesWithConstraints](/deployedge/microsoft-edge-policies#cacertificateswithconstraints) - TLS certificates that should be trusted by Microsoft Edge for server authentication with constraints
- [CADistrustedCertificates](/deployedge/microsoft-edge-policies#cadistrustedcertificates) - TLS certificates that should be distrusted by Microsoft Edge for server authentication
- [CAHintCertificates](/deployedge/microsoft-edge-policies#cahintcertificates) - TLS certificates that aren't trusted or distrusted but can be used in path-building for server authentication
- [CAPlatformIntegrationEnabled](/deployedge/microsoft-edge-policies#caplatformintegrationenabled) - Use user-added TLS certificates from platform trust stores for server authentication
- [DataURLWhitespacePreservationEnabled](/deployedge/microsoft-edge-policies#dataurlwhitespacepreservationenabled) - DataURL Whitespace Preservation for all media types
- [EdgeSidebarAppUrlHostForceList](/deployedge/microsoft-edge-policies#edgesidebarappurlhostforcelist) - Control which apps are forced to be shown in Microsoft Edge sidebar
- [PdfViewerOutOfProcessIframeEnabled](/deployedge/microsoft-edge-policies#pdfvieweroutofprocessiframeenabled) - Use out-of-process iframe PDF Viewer
- [SeamlessWebToBrowserSignInEnabled](/deployedge/microsoft-edge-policies#seamlesswebtobrowsersigninenabled) - Seamless Web To Browser Sign-in Enabled
- [WebToBrowserSignInEnabled](/deployedge/microsoft-edge-policies#webtobrowsersigninenabled) - Web To Browser Sign-in Enabled

#### Obsoleted policies

- [CopilotCDPPageContext](/deployedge/microsoft-edge-policies#copilotcdppagecontext) - Control Copilot with Commercial Data Protection access to page context for Microsoft Entra ID profiles (obsolete)
- [CSSCustomStateDeprecatedSyntaxEnabled](/deployedge/microsoft-edge-policies#csscustomstatedeprecatedsyntaxenabled) - Controls whether the deprecated :--foo syntax for CSS custom state is enabled (obsolete)
- [LegacySameSiteCookieBehaviorEnabledForDomainList](/deployedge/microsoft-edge-policies#legacysamesitecookiebehaviorenabledfordomainlist) - Revert to legacy SameSite behavior for cookies on specified sites (obsolete)

> [!NOTE]
>For the latest web platform features and updates, see [Microsoft Edge 133 web platform release notes (Feb. 2025).](/microsoft-edge/web-platform/release-notes/133)

## Version 132.0.2957.140: January 30, 2025

Fixed various bugs and performance issues.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#january-30-2025).

## Version 132.0.2957.127: January 24, 2025

Fixed various bugs and performance issues.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#january-24-2025).

## Version 132.0.2957.115: January 17, 2025

Fixed various bugs and performance issues, Dev channel updates, feature updates, policy updates, and site compatibility impacting changes.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#january-17-2025).

### Dev Channel updates

The following Dev channel updates preceded this Stable channel release. The following Dev notes provide detailed information about the changes in each release.

- [Dev Channel update to 132.0.2917.0 is live. | Microsoft Community Hub](https://techcommunity.microsoft.com/discussions/edgeinsiderannouncements/dev-channel-update-to-132-0-2917-0-is-live-/4283359)
- [Dev Channel update to 132.0.2931.1 is live. | Microsoft Community Hub](https://techcommunity.microsoft.com/discussions/edgeinsiderannouncements/dev-channel-update-to-132-0-2931-1-is-live-/4288628)
- [Dev Channel update to 132.0.2945.0 is live. | Microsoft Community Hub](https://techcommunity.microsoft.com/discussions/edgeinsiderannouncements/dev-channel-update-to-132-0-2945-0-is-live-/4296080)
- [Dev Channel update to 132.0.2957.11 is live. | Microsoft Community Hub](https://techcommunity.microsoft.com/discussions/edgeinsiderannouncements/dev-channel-update-to-132-0-2957-11-is-live-/4342194)

### Fixes

- Fixed an issue on macOS that caused rendering issues and missing text when viewing certain PDF files containing Japanese fonts.

### Feature updates

- **Intune policies in the Microsoft Edge management service.** Admins now can set Intune policies via the Microsoft Edge management service, alongside the existing cloud policies. This ability lets admins deploy both browser policies in the cloud and Intune policies from a single pane, making it easy to keep users safe and the browser workflow streamlined. This feature comes along with a new policy creation wizard that streamlines the creation process into a comprehensive, step-by-step flow. Note: This experience is in public preview and can be accessed by opting in to targeted release in the Microsoft 365 admin center.

- **Version monitoring in the Edge management service.** The Edge management service offers a single view of all managed Edge instances with their update status and possible actions to take. For out-of-date devices, you can easily schedule updates or notify users to update their browsers to avoid workflow interruptions. Note: This experience is in public preview and can be accessed by opting in to targeted release in the Microsoft 365 admin center.

- **Shopping Product Tracking.** Track product prices easily with a new experience in the Edge Address Bar that appears on the product detail page. Users can track prices quickly and are notified when there's a price drop on that product and save more. Administrators can control the availability of Shopping in Edge using the [EdgeShoppingAssistantEnabled](/deployedge/microsoft-edge-policies#edgeshoppingassistantenabled) policy. Note: This feature is a controlled feature rollout. If you don't see this feature, check back as we continue our rollout.
 
- **New password manager policy.** The [DeletingUndecryptablePasswordsEnabled](/deployedge/microsoft-edge-policies#deletingundecryptablepasswordsenabled) policy controls whether the built-in password manager can delete undecryptable passwords from its database. This policy is required to restore the full functionality of the built-in password manager, but it might cause permanent data loss. Undecryptable password values won't become decryptable on their own. If fixing them is possible, it usually requires complex user actions.

- **PromotionalTabsEnabled policy deprecation.** [The PromotionalTabsEnabled](/deployedge/microsoft-edge-policies#promotionaltabsenabled) policy is deprecated in Microsoft Edge version 132 and will be obsolete in a future Microsoft Edge version. Administrators can use the [ShowRecommendationsEnabled](/deployedge/microsoft-edge-policies#promotionaltabsenabled) policy instead.
 
- **Allow enterprise users to view XFA PDFs using IE Mode.** Enterprise customers can view XFA PDFs in Microsoft Edge using IE mode through either the [ViewXFAPDFInIEModeAllowedOrigins](/deployedge/microsoft-edge-policies#viewxfapdfiniemodeallowedorigins) or [ViewXFAPDFInIEModeAllowedFileHash](/deployedge/microsoft-edge-policies#viewxfapdfiniemodeallowedfilehash) policy. This change is available in the new PDF viewer on Microsoft Edge.
 
- **Deprecation of Microsoft Edge Support page.** To improve end user experience, edge://support is being deprecated. The information found on edge://support is available on other pages: *edge://version, edge://metrics-internals, edge://extensions, and edge://policy.*

- **Full Favorites Bar available in Workspaces.**  Workspaces now display a user's full set of favorites in the Favorites Bar, with a dedicated workspace folder accessible from the bar. Previously when in a workspace, a user's existing Favorites Bar wasn't easily accessible and instead only the workspace favorites folder was visible.  Users can control the behavior by **modifying #edge-workspace-favorites-bar** in edge://flags.

### Policy updates

#### New policies

- [AdHocCodeSigningForPWAsEnabled](/deployedge/microsoft-edge-policies#adhoccodesigningforpwasenabled) - Native application signing during Progressive Web Application installation
- [AutomaticFullscreenAllowedForUrls](/deployedge/microsoft-edge-policies#automaticfullscreenallowedforurls) - Allow automatic full screen on specified sites
- [AutomaticFullscreenBlockedForUrls](/deployedge/microsoft-edge-policies#automaticfullscreenblockedforurls) - Block automatic full screen on specified sites
- [CreatePasskeysInICloudKeychain](/deployedge/microsoft-edge-policies#createpasskeysinicloudkeychain) - Control whether passkey creation will default to iCloud Keychain
- [DeletingUndecryptablePasswordsEnabled](/deployedge/microsoft-edge-policies#deletingundecryptablepasswordsenabled) - Enable deleting undecryptable passwords
- [EdgeAutofillMlEnabled](/deployedge/microsoft-edge-policies#edgeautofillmlenabled) - Machine learning powered autofill suggestions
- [GenAILocalFoundationalModelSettings](/deployedge/microsoft-edge-policies#genailocalfoundationalmodelsettings) - Settings for GenAI local foundational model
- [IPv6ReachabilityOverrideEnabled](/deployedge/microsoft-edge-policies#ipv6reachabilityoverrideenabled) - Enable IPv6 reachability check override
- [PersonalizeTopSitesInCustomizeSidebarEnabled](/deployedge/microsoft-edge-policies#personalizetopsitesincustomizesidebarenabled) - Personalize my top sites in Customize Sidebar enabled by default
- [SelectParserRelaxationEnabled](/deployedge/microsoft-edge-policies#selectparserrelaxationenabled) - Controls whether the new HTML parser behavior for the `<select>` element is enabled
- [ViewXFAPDFInIEModeAllowedFileHash](/deployedge/microsoft-edge-policies#viewxfapdfiniemodeallowedfilehash)- View XFA-based PDF files using IE Mode for allowed file hash.
- [ViewXFAPDFInIEModeAllowedOrigins](/deployedge/microsoft-edge-policies#viewxfapdfiniemodeallowedorigins) - View XFA-based PDF files using IE Mode for allowed file origin.

#### Deprecated policies

- [InsecureFormsWarningsEnabled](/deployedge/microsoft-edge-policies#insecureformswarningsenabled) - Enable warnings for insecure forms (deprecated)
- [LegacySameSiteCookieBehaviorEnabledForDomainList](/deployedge/microsoft-edge-policies#legacysamesitecookiebehaviorenabledfordomainlist) - Revert to legacy SameSite behavior for cookies on specified sites (deprecated)
- [MutationEventsEnabled](/deployedge/microsoft-edge-policies#mutationeventsenabled) - Enable deprecated/removed Mutation Events (deprecated)
- [PromotionalTabsEnabled](/deployedge/microsoft-edge-policies#promotionaltabsenabled)- Enable full-tab promotional content (deprecated)

#### Obsoleted policies

- [BlockTruncatedCookies](/deployedge/microsoft-edge-policies#blocktruncatedcookies) - Block truncated cookies (obsolete)
- [CertificateTransparencyEnforcementDisabledForLegacyCas](/deployedge/microsoft-edge-policies#certificatetransparencyenforcementdisabledforlegacycas) - Disable Certificate Transparency enforcement for a list of legacy certificate authorities (obsolete)

#### Site compatibility impacting changes

>[!NOTE]
>Portions of this release note are modifications based on work created and shared by Chromium.org and used according to terms described in the [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/)
>
- **Removal of old Headless from the Edge binary.**  Running Edge with `--headless=old` no longer launches the old Headless mode, and instead prints the following log message: Old Headless mode has been removed from the Chrome binary. Please use the [new Headless mode](https://developer.chrome.com/docs/chromium/headless) or the chrome-headless-shell which is a standalone implementation of the [old Headless mode](https://developer.chrome.com/blog/chrome-headless-shell).

- **CSS Anchor Positioning: allow `anchor-size()` in inset and margin properties.** Originally, `anchor-size()` was only allowed in sizing properties. The specification now allows `anchor-size()` in insets and margins as well.

- **CSS sideways writing modes.** Support of `sideways-rl` and `sideways-lr` keywords for the `writing-mode` CSS property. `sideways-rl` and `sideways-lr` are helpful to write non-CJK text vertically. They don't have behaviors favorable for CJK languages unlike `vertical-rl` and `vertical-lr`.

- **Dialog toggle events.** This change incorporates the same `ToggleEvent` that popovers dispatch, but for `<dialog>` elements: when `showModal` or `show` is called, `<dialog>` dispatches a `ToggleEvent` with `newState=open`. When a `<dialog>` is closed (using the form, button, or close watcher) it should dispatch a `ToggleEvent` with `newState=closed`.

  Previously, to detect when a `<dialog>` opens a mutation observer had to be registered to check for open.

- **Element Capture.** Given a video `MediaStreamTrack` obtained through pre-existing means to initiate tab-capture, Element Capture allows mutating the track to only capture a subtree of the DOM starting at a given Element.

  The API bears some resemblance to the Region Capture API, but affords greater flexibility for applications, because occluding and occluded content are both excluded from the capture.

- **FedCM authorization features.** This bundles a few features that Identity Providers (IdP) can use to implement authorization flows such as letting a user grant access to their calendar to a Relying Party (RP). Specifically:

  - The IdP needs to be able to show a custom prompt for the permission (continuation API).
  - The RP needs an extensible way to communicate to the IdP what it wants access to (parameters API).
  - The RP needs to be able to customize or suppress the text referring to the IdP sharing "name, email address, and profile picture" because in this situation they're asking for different information (fields API).
  - The IdP might want to use a different endpoint to implement the authorization flow (multiple configURLs).
  - Certain accounts may only be eligible for one of the authentication and authorization flows and so there needs to be a way to show different accounts in the two flows (account labels API).

- **FedCM Mode API and Use Other Account API.** Two new extensions for FedCM:

  - **Mode**: The `active` mode allows websites to call FedCM inside a button click (for example, selecting a **Sign-in to IdP** button), which requires FedCM to guarantee it always responds with a visible user interface. Calling the FedCM API in *active mode* takes users to sign in to the Identity Provider (IdP) when users are logged-out. Also, because the active mode is called within an explicit user gesture, the UI is also more prominent (for example, centered and modal) compared to the UI from the passive mode (which doesn't require a user gesture requirement and can be called on page load).
  - **Use Other Account**: With this extension, an IdP can allow users to sign in to other accounts.

- **Fetch: `Request.bytes()` and `Response.bytes()`.** Add a `bytes()` method to the `Request` and `Response` interfaces, which returns a promise that resolves with a Uint8Array. While `Request` and `Response` have an `arrayBuffer()` method, it’s not possible to read directly from a buffer. A view such as a `Uint8Array` must be created to read it. The `bytes()` method improves the ergonomics of getting the body of Request and Response.

- **Ignore Strict-Transport-Security for localhost.** `Strict-Transport-Security` (STS) response headers can cause problems for localhost web servers because STS applies host-wide, across all ports. This causes compatibility problems for web developers testing locally. It also affects end-users who use software packages that commonly start localhost web servers for ephemeral reasons. For example, communication of an auth token from a web sign-in to a local software package. If one local listener sets `Strict-Transport-Security` on a localhost response, it's applied to all subsequent localhost requests regardless of port.

  Edge 132 resolves this problem by ignoring `Strict-Transport-Security` headers on responses from localhost URLs.
  
- **Keyboard focusable scroll containers.** The rollout of this feature (from Edge 130) was stopped due to an accessibility regression. This issue is fixed and the feature continues to rollout with Edge 132. [KeyboardFocusableScrollersEnabled]( /deployedge/microsoft-edge-policies#keyboardfocusablescrollersenabled) is the policy for this feature.

- **Private State Token API Permissions Policy default allowlist wildcard.** Access to the Private State Token API is gated by Permissions Policy features. Edge 132 updates the default allowlist for both `private-state-token-issuance` and `private-state-token-redemption` features from `self` to `*` (wildcard).

- **`PushMessageData::bytes()`.** The `PushMessageData` interface mimics the `Body` interface, which was amended earlier this year with a new `bytes()` method, following the principle that APIs should generally vend byte buffers as `Uint8Arrays`. Edge 132 realigns with the `Body` interface by providing the `bytes()` accessor on the `PushMessageData` interface as well.

- **Saved queries in `sharedStorage.selectURL`.** `sharedStorage.selectURL()` now lets queries be saved and reused on a per-page basis. Two per-page-load budgets are charged the first time a saved query is run but not for subsequent runs of the saved query during the same page-load. This change is accomplished with a `savedQuery` parameter in the options for `selectURL()` that names the query.

- **Throw exception for popovers and dialogs in non-active documents.** Previously calling `showPopover()` or `showModal()` on a popover or dialog that resides within an inactive document would silently fail. No exception was thrown, but since the document is inactive, no popover or dialog would be shown. As of Edge 132, these situations now throw `InvalidStateError`.

- **WebAuthn Signal API.** Allows WebAuthn relying parties to signal information about existing credentials back to credential storage providers, so that incorrect or revoked credentials can be updated or removed from provider and system UI.

- **WebGPU: 32-bit float textures blending.** The `float32-blendable` GPU feature makes GPU textures with formats `r32float`, `rg32float`, and `rgba32float` blendable.

- **WebGPU: Expose GPUAdapterInfo from GPUDevice.** The GPUDevice `adapterInfo` attribute exposes the same `GPUAdapterInfo` as the `GPUAdapter` object.

- **WebGPU: Texture view usage.** Adds an optional field to WebGPU texture view creation to request a subset of the usage flags from the source texture.

  By default, texture view usage inherits from the source texture but there are view formats that can be incompatible with the full set of inherited usages. Adding a usage field to texture view creation allows the user request a subset of the source texture's usages that are valid with the view format and specific to their intended usage of the texture view.

  WebGPU implementations can also optimize the creation of low level resources and improve performance when using views with more specialized usage flags.

- **New origin trials: Document-Isolation-Policy.** The **Document-Isolation-Policy** lets a document enable `crossOriginIsolation` for itself, without having to deploy COOP or COEP, and regardless of the `crossOriginIsolation` status of the page. The policy is backed by process isolation. Additionally, the document non-CORS cross-origin subresources will either be loaded without credentials or will need to have a CORP header.

- **New origin trials: Explicit Compile Hints with Magic Comments.** This feature lets you attach information about which functions should be eager parsed and compiled in JavaScript files. The information is encoded as magic comments.

- **`navigator.storage` no longer an EventTarget.** `navigator.storage` was made an `EventTarget` for the Storage Pressure Event, which never made it past the prototype phase. This dead code is being removed and as a result, `navigator.storage` will no longer extend `EventTarget`.

- **Remove Prefixed HTMLVideoElement Fullscreen APIs.** The prefixed HTMLVideoElement fullscreen APIs have been deprecated from Edge.

  They were replaced by the `Element.requestFullscreen()` API. As of 2024, most browsers have had support for the unprefixed APIs for a few years now.

  Edge 132 removes the following from `HTMLVideoElement`:

  - The `webkitSupportsFullscreen` attribute.
  - The `webkitDisplayingFullscreen` attribute.
  - The `webkitEnterFullscreen()` method.
  - The `webkitExitFullscreen()` method. Note the different capitalization of the "S" in FullScreen.
  - The `webkitEnterFullScreen()` method.
  - The `webkitExitFullScreen()` method.

  These methods are now only aliases for the modern API. Their use has declined steadily over the years.

## Version 131.0.2903.147: January 10, 2025

Fixed various bugs and performance issues.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#January-10-2025).

## Version 131.0.2903.146: January 10, 2025

Fixed various bugs and performance issues.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#January-10-2025).

## Version 130.0.2849.142: January 10, 2025

Fixed various bugs and performance issues for Extended Stable Channel.

## Version  131.0.2903.112: December 19, 2024

Fixed various bugs and performance issues.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#december-19-2024).

## Version 130.0.2849.123: December 19, 2024

Fixed various bugs and performance issues for Extended Stable Channel.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#december-19-2024).

## Version 130.0.2849.116: December 13, 2024

Fixed various bugs and performance issues for Extended Stable Channel.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#december-12-2024).

## Version  131.0.2903.99: December 12, 2024

Fixed various bugs and performance issues.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#december-12-2024).

## Version  131.0.2903.86: December 5, 2024

Fixed various bugs and performance issues.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#december-5-2024).

## Version 130.0.2849.108: December 5, 2024

Fixed various bugs and performance issues for Extended Stable channel.

## Version  131.0.2903.70: November 25, 2024

Fixed various bugs and performance issues.

### Fixes

- Fixed an issue on Windows that caused rendering issues and missing text when viewing certain PDF files containing Japanese fonts.

## Version 131.0.2903.63: November 21, 2024

Fixed various bugs and performance issues.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#november-21-2024).

### Fixes
  
- Fixed an issue which prevented the "Delete browsing data" dialog window from closing after clicking the "Clear now" button. 

## Version 131.0.2903.51: November 15, 2024

Fixed various bugs and performance issues.

## Version 130.0.2849.99: November 14, 2024

Fixed various bugs and performance issues for Extended Stable release.

## Version 131.0.2903.48: November 14, 2024

Fixed various bugs and performance issues, Dev channel updates, feature updates, policy updates, and site compatibility impacting changes.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#november-14-2024).

### Announcement

Microsoft Edge WebView2 Runtime will no longer appear in the Installed Apps list in Windows Settings because it's a persistent system component.

### Dev Channel updates

The following Dev channel updates preceded this Stable channel release. The following Dev notes provide detailed information about the changes in each release.

- [Dev Channel update to 131.0.2863.0 is live. - Microsoft Community Hub](https://techcommunity.microsoft.com/discussions/edgeinsiderannouncements/dev-channel-update-to-131-0-2863-0-is-live-/4260359)
- [Dev Channel update to 131.0.2875.0 is live. - Microsoft Community Hub](https://techcommunity.microsoft.com/discussions/edgeinsiderannouncements/dev-channel-update-to-131-0-2875-0-is-live-/4267839)
- [Dev Channel update to 131.0.2889.0 is live. - Microsoft Community Hub](https://techcommunity.microsoft.com/discussions/edgeinsiderannouncements/dev-channel-update-to-131-0-2889-0-is-live-/4273465)
- [Dev Channel update to 131.0.2903.5 is live. - Microsoft Community Hub](https://techcommunity.microsoft.com/discussions/edgeinsiderannouncements/dev-channel-update-to-131-0-2903-5-is-live-/4277981)

### Feature updates

- **Cancel dialog for `beforeunload` event.** Microsoft Edge changed the behavior of the canceled dialog for the `beforeunload` event. Calling `event.preventDefault` in a `beforeunload` event handler won't prevent the dialog from being shown. Instead, `event.returnValue = ''` needs to be called in the `beforeunload` event handler to prevent the canceled dialog. The [BeforeunloadEventCancelByPreventDefaultEnabled](/deployedge/microsoft-edge-policies?branch=main#beforeunloadeventcancelbypreventdefaultenabled) policy is obsolete and no longer works after Microsoft Edge version 130.

- **Changes to Kyber.** The Kyber algorithm was standardized with minor technical changes and renamed to the Module Lattice Key Encapsulation Mechanism (ML-KEM). ML-KEM is implemented in the BoringSSL cryptography library, which allows for it to be deployed and utilized by services that depend on this library.

  The changes to the final version of ML-KEM make it incompatible with the previously deployed version of Kyber. Due to this incompatibility the following changes in Microsoft Edge will be made:

  - Edge switches from supporting Kyber to ML-KEM.
  - Edge offers a key share prediction for hybrid ML-KEM (codepoint 0x11EC).
  - The `PostQuantumKeyAgreementEnabled` flag and the [PostQuantumKeyAgreementEnabled](/deployedge/microsoft-edge-policies#postquantumkeyagreementenabled) policy applies to Kyber and ML-KEM. Note: The [PostQuantumKeyAgreementEnabled](/deployedge/microsoft-edge-policies#postquantumkeyagreementenabled) policy is scheduled for removal in Edge version 141.
  - Edge will no longer support hybrid Kyber (codepoint 0x6399).

- **New sidebar policy.** The [EdgeSidebarAppUrlHostAllowList](/deployedge/microsoft-edge-policies#edgesidebarappurlhostallowlist) policy allows admins to define a list of sites, based on URL patterns, that are not subject to the [EdgeSidebarAppUrlHostBlockList](/deployedge/microsoft-edge-policies#edgesidebarappurlhostblocklist). When the policy is configured, the apps listed in the allow list can be opened in sidebar even if they're listed in the blocklist. For more information, see [Manage the sidebar in Microsoft Edge](/deployedge/microsoft-edge-sidebar#allow-specific-sidebar-apps-except-search-using-urls).

- **Support for Microsoft Purview Information Protection label for Office Online documents.** Microsoft Edge for Business now natively supports enforcing data loss prevention (DLP) controls via Microsoft Information Protection (MIP) sensitivity labels in Word, Excel, and PowerPoint documents in Office online. This support closes the document protection gap in browser scenarios for commercial users.  The following leak controls are now natively supported in the browser:
   - Copy
   - Debugging Tools 
   - Export
   - Extract
   - Paste
   - Print
   - Save as (PDF,Webpage)
   - Screenshots

For more information about how to enable, [see Protect Office documents with Microsoft Purview Information Protection labeling | Microsoft Learn.](/deployedge/microsoft-edge-management-service-office-mip)

### Policy updates

#### New policies

- [EdgeSidebarAppUrlHostAllowList](/deployedge/microsoft-edge-policies#edgesidebarappurlhostallowlist) - Allow specific apps to be opened in Microsoft Edge sidebar
- [PrivateNetworkAccessRestrictionsEnabled](/deployedge/microsoft-edge-policies#privatenetworkaccessrestrictionsenabled) - Specifies whether to apply restrictions to requests to more private network endpoints

#### Deprecated policies

- [NewBaseUrlInheritanceBehaviorAllowed](/deployedge/microsoft-edge-policies#newbaseurlinheritancebehaviorallowed) - Allows enabling the feature NewBaseUrlInheritanceBehavior (deprecated)
- [RSAKeyUsageForLocalAnchorsEnabled](/deployedge/microsoft-edge-policies#rsakeyusageforlocalanchorsenabled) - Check RSA key usage for server certificates issued by local trust anchors (deprecated)
- [UserAgentClientHintsGREASEUpdateEnabled](/deployedge/microsoft-edge-policies#useragentclienthintsgreaseupdateenabled) - Control the User-Agent Client Hints GREASE Update feature (deprecated)

#### Obsoleted policies

- [BeforeunloadEventCancelByPreventDefaultEnabled](/deployedge/microsoft-edge-policies#beforeunloadeventcancelbypreventdefaultenabled) - Control the behavior for the cancel dialog produced by the beforeunload event (obsolete)
- [SignInCtaOnNtpEnabled](/deployedge/microsoft-edge-policies#signinctaonntpenabled) - Enable sign in click to action dialog (obsolete)

### Site compatibility impacting changes

> [!NOTE]
> Portions of this release note are modifications based on work created and shared by Chromium.org and used according to terms described in the [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).

- **CSS Anchor Positioning: `anchor-scope`.** The `anchor-scope` property allows limiting the visibility of anchor names to a given subtree.

- **CSS `font-variant-emoji`.** The `font-variant-emoji` CSS property provides a way to control between colored (emoji-style) and monochromatic (text-style) emoji glyphs. This method can be also done by adding an emoji Variation Selector, specifically U+FE0E for text and U+FE0F for emoji, after each emoji codepoint.

- **CSS highlight inheritance.** With CSS highlight inheritance, the CSS highlight pseudo-classes, such as `::selection` and `::highlight`, inherit their properties through the pseudo highlight chain, rather than the element chain. The result is a more intuitive model for inheritance of properties in highlights.

- **Improvements to styling structure of `<details>` and `<summary>` elements.** Support more CSS styling for the structure of `<details>` and `<summary>` elements to allow these elements to be used in more cases where disclosure widgets or accordion widgets are built on the web. In particular, this change removes restrictions that prevented setting the display property on these elements, and adds a `::details-content` pseudo-element to style the container for the part that expands and collapses.

- **`@page` margin boxes.** Add support for page margin boxes, when printing a web document, or exporting it as PDF.

  The `@page` margin boxes let you define the contents in the margin area of a page, for example to provide custom headers and footers, rather than using the built-in headers and footers generated by the browser.

  A margin box is defined using an at-rule inside a CSS `@page` rule. The appearance and the contents of a margin box are specified with CSS properties inside the `@page` rule, including the `content` property. Counters are also supported, for page numbering. The specification defines two special counter names: `page` for the current page number and `pages` for the total number of pages.

- **@property support `<string>` syntax.** Support for `<string>` syntax component name for registered custom properties.

- **Support `currentcolor` in relative color syntax.** Allow relative colors in CSS (using the `from` keyword) to use `currentcolor` as a base. This support lets you set complementary colors, based on an element's text color, for that element's borders, shadows, or backgrounds.

  This feature also includes use cases where color functions are nested with a dependency on `currentcolor`, for example: `color-mix (in srgb, rgb(from currentcolor r g b), white)) or rgb(from rgb(from currentcolor 1 g b) b g r)`.

- **Support external SVG resources for `clip-path`, `fill`, `stroke`, and `marker-*` properties.** This feature adds support for external references for clip paths, markers, and paint servers (for the `fill` and `stroke` properties). For example, `clip-path: url("resources.svg#myPath")`.

- **Direct Sockets API.** Allows Isolated Web Apps to establish direct transmission control protocol (TCP) and user datagram protocol (UDP) communications with network devices and systems as well as listen to and accept incoming connections.

- **Exempt `Speculation-Rules` header from CSP restrictions.** Updates the integration between speculation rules and CSP so that CSP only applies to `<script type=speculationrules>`, and not to the `Speculation-Rules` header. CSP's script policies are meant to protect against injection of scripts into HTML, and the CSP threat model doesn't relate to HTTP headers. This approach allows easier deployment of speculation rules from CDNs and other edge servers.

- **FedCM as a trust signal for the Storage Access API.** Reconciles the FedCM and Storage Access APIs by making a prior FedCM grant a valid reason to automatically approve a storage access request.

  When a user grants permission to use their identity with a third-party identity provider (IdP) on a relying party (RP), many IdPs require third-party cookies to function correctly and securely. This proposal aims to satisfy that requirement in a private and secure manner by updating the Storage Access API (SAA) permission checks to not only accept the permission grant given by a storage access prompt, but also the permission grant given by a FedCM prompt.

  A key property of this mechanism is limiting the grant to cases explicitly allowed by the RP with the FedCM permissions policy, enforcing a per-frame control for the RP and preventing passive surveillance by the IdP beyond the capabilities that FedCM already grants.

- **COOP value `noopener-allow-popups`.** Some origins can contain different applications with different levels of security requirements. In those cases, it can be beneficial to prevent scripts running in one application from being able to open and script pages of another same-origin application.

  In such cases, it can be beneficial for a document to ensure its opener can't script it, even if the opener document is a same-origin one. The `noopener-allow-popups` Cross-Origin-Opener-Policy value lets documents define that behavior.

- **Select parser relaxation.** This change makes the HTML parser allow more tags in `<select>` besides `<option>`, `<optgroup>`, and `<hr>`.

  This change is in support of the customizable `<select>` feature but is being shipped first because it can be done separately and has some compat risk.

- **WebGPU: Clip distances.** Adds the optional GPU feature `clip-distances` that allows setting user-defined clip distances in vertex shader outputs. This technique is useful for the applications that need to clip all vertices in a scene that are beyond a user-defined plane, such as many CAD applications.

- **WebGPU: `GPUCanvasContext getConfiguration()`**. Once `GPUCanvasContext configure()` is called with a configuration dictionary, the `GPUCanvasContext getConfiguration()` method can be used to check the canvas context configuration. It includes GPU `device`, `format`, `usage`, `viewFormats`, `colorSpace`, `toneMapping`, and `alphaMode` members. As discussed in [issue 4828](https://github.com/gpuweb/gpuweb/issues/4828), web apps can use it to detect whether HDR canvas is supported in WebGPU.

- **WebHID on dedicated workers.** Enables WebHID inside dedicated worker contexts. This lets the performance of heavy I/O and processing of data from a HID device on a separate thread, helping to reduce the performance impact on the main thread.

- **WebRTC `RTCRtpEncodingParameters.scaleResolutionDownTo`.** An API that configures WebRTC encoders to scale input frames if they're greater than the specified `maxWidth` and `maxHeight`. This API is similar to `scaleResolutionDownBy` except that resolution constraints are expressed in absolute terms (for example, 640x360) as opposed to relative terms (for example, scale down by 2), avoiding race conditions related to changing input frame size on the fly.

- **Remove the CSS Anchor Positioning property `inset-area`.** With the CSS Working Group resolution on renaming the `inset-area` property to `position-area`, this removal cleans up the implementation for a standards compliant feature.

- **Remove non-standard GPUAdapter `requestAdapterInfo()` method.** The WebGPU Working Group decided it was impractical for `requestAdapterInfo()` to trigger a permission prompt so they removed that option and replaced it with the GPUAdapter `info` attribute so that web developers can get the same `GPUAdapterInfo` value synchronously.

<!----------------end changes------------------------------------>
## Version 130.0.2849.80: November 7, 2024

Fixed various bugs and performance issues.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#november-7-2024).

## Version 130.0.2849.68: October 31, 2024

Fixed various bugs and performance issues, improved reliability.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#october-31-2024).

### Improved reliability

- Fixed a renderer crash (STATUS_BREAKPOINT) that occurred when using some sites with web contents accessibility enabled.

## Version 130.0.2849.56: October 24, 2024

Fixed various bugs and performance issues.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#october-24-2024).

### Fixes

- Fixed an issue which prevented some browser extensions using the `chrome.storage.managed` API from functioning correctly.

## Version 130.0.2849.52: October 22, 2024

Fixed various bugs and performance issues, improved reliability.

### Improved reliability

- Fixed a browser crash that occurred on startup in On-premises environments when creating a new Microsoft Edge profile.

## Version 130.0.2849.46: October 17, 2024

Fixed various bugs and performance issues, Dev channel updates, announcements, feature updates, site compatibility impacting changes, and policy updates.

> [!NOTE]
> Portions of this release note are modifications based on work created and shared by Chromium.org and used according to terms described in the [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#october-17-2024).

### Dev Channel updates

The following Dev channel updates preceded this Stable channel release. The following Dev notes provide detailed information about the changes in each release.

- [Dev Channel update to 130.0.2808.0 is live. - Microsoft Community Hub](https://techcommunity.microsoft.com/t5/articles/dev-channel-update-to-130-0-2808-0-is-live/m-p/4237117)
- [Dev Channel update to 130.0.2821.1 is live. - Microsoft Community Hub](https://techcommunity.microsoft.com/t5/articles/dev-channel-update-to-130-0-2821-1-is-live/m-p/4242634)
- [Dev Channel update to 130.0.2835.2 is live. - Microsoft Community Hub](https://techcommunity.microsoft.com/t5/articles/dev-channel-update-to-130-0-2835-2-is-live/m-p/4250520)
- [Dev Channel update to 130.0.2849.1 is live. - Microsoft Community Hub](https://techcommunity.microsoft.com/t5/articles/dev-channel-update-to-130-0-2849-1-is-live/m-p/4255515)

### Fixes

- Fixed an issue that prevented the briefcase icon from appearing on the *edge://settings/sidebar* page when Edge Bar was disabled using the [StandaloneHubsSidebarEnabled](/deployedge/microsoft-edge-policies#standalonehubssidebarenabled) policy.

- Fixed an issue that caused rendering issues on some SharePoint sites.

- Fixed an issue where a "Can't update Microsoft Edge" dialog was mistakenly shown for managed Windows devices.

### Announcements

- **Live Captions.** The [LiveCaptionsAllowed](/deployedge/microsoft-edge-policies#livecaptionsallowed) policy was available since Microsoft Edge version 103 but this feature isn't generally available. Clients that have the [ExperimentationAndConfigurationServiceControl](/deployedge/microsoft-edge-policies#experimentationandconfigurationservicecontrol) policy set to 'FullMode' might receive the feature before broad availability. Broad availability will be announced via Microsoft Edge release notes.

- **Cancel dialog for `beforeunload` event.** Microsoft Edge is changing the behavior of the cancel dialog for the `beforeunload` event in Microsoft Edge version 131. Starting in version 131, calling `event.preventDefault` in a `beforeunload` event handler won't prevent the dialog from being shown. Instead, `event.returnValue = ''` needs to be called in the `beforeunload` event handler to prevent the cancel dialog. The [BeforeunloadEventCancelByPreventDefaultEnabled](/deployedge/microsoft-edge-policies#beforeunloadeventcancelbypreventdefaultenabled) policy is being obsoleted and will no longer work after Microsoft Edge version 130.

### Feature updates

- **Token Binding.** Token Binding uses cryptographic certificates on both ends of the TLS connection in an attempt to close the security gap of bearer tokens, which might be lost or stolen. Token Binding is deprecated in Microsoft Edge version 130. Also, the [AllowTokenBindingForUrls](/deployedge/microsoft-edge-policies#allowtokenbindingforurls) policy is now obsolete.

- **Copilot browser Context Policies.** The [EdgeEntraCopilotPageContext](/deployedge/microsoft-edge-policies#edgeentracopilotpagecontext) policy will be available starting from Microsoft Edge version 130 and will replace the [CopilotCDPPageContext](/deployedge/microsoft-edge-policies#copilotcdppagecontext) policy. The [CopilotCDPPageContext](/deployedge/microsoft-edge-policies#copilotcdppagecontext) policy is deprecated in Microsoft Edge version 130 and will be obsolete in Edge 133.

- **Elevating top settings and improving settings page navigability.** To make finding browser settings more efficient, Microsoft Edge is introducing three navigation improvements to Edge Settings. We aren’t changing the functionality of any setting, and all the settings stay on the same page as they are today but are behind clickable sections. These changes are as follows.

  - Introduce quick access to the most used Settings actions on the first place users land when entering Edge Settings (the Profiles page). Clicking the button with the name of the setting navigates users directly to its location.

  - Make densely populated Settings pages (such as *Privacy, search, and services*, *Appearance*, *Cookies and site permissions*, *System and performance*) easier to navigate by introducing quick access to the most used actions located on that page. Clicking the button with the name of the setting takes users directly to its location.

  - For these densely populated pages, each lengthy section of settings will be a clickable "table of contents" with descriptive subtexts. This helps users locate settings directly and avoid unnecessary scrolling.

  **Note:** This feature is a controlled feature rollout. If you don't see this feature, check back as we continue our rollout.

- **Edge on macOS now seamlessly opens links in Teams.** When Microsoft Edge is configured as the browser to open web links in Teams, then links in Teams chat will be opened through Edge, and Edge launches in the profile that matches with the authenticated profile, users can benefit from a seamless browsing experience that integrates their identity and user data across Microsoft apps. Administrators can control the availability of this feature using the "Choose Which Browser Opens Web Links" Microsoft 365 policy. **Note:** This feature is a controlled feature rollout. If you don't see this feature, check back as we continue our rollout.

### Site compatibility impacting changes

- **Compression dictionary transport with shared Brotli and shared Zstandard.** This feature adds support for using designated previous responses, as an external dictionary for content encoding compressing responses with Brotli or Zstandard.

  Enterprises might experience potential compatibility issues with enterprise network infrastructure that intercepts HTTPS traffic and is sensitive to unknown content encodings. The [CompressionDictionaryTransportEnabled](/deployedge/microsoft-edge-policies#compressiondictionarytransportenabled) policy is available to turn off the compression dictionary transport feature.

- **Keyboard focusable scroll containers.** This feature improves accessibility by making scroll containers focusable using sequential focus navigation. Today, the tab key doesn't focus scrollers unless tabIndex is explicitly set to 0 or more.

  By making scrollers focusable by default, users without a mouse can now focus clipped content using tab and arrow keys. This behavior is enabled only if the scroller does not contain any keyboard-focusable children. This logic is necessary so there are no regressions for existing focusable elements that might exist within a scroller like a \<textarea\>.

  If more time is needed to adjust to this new feature, the [KeyboardFocusableScrollersEnabled](/deployedge/microsoft-edge-policies#keyboardfocusablescrollersenabled) policy is available from Edge 128.

- **Support non-special scheme URLs.** [Non-special scheme URLs](https://url.spec.whatwg.org/#is-special) are now supported, for example, *git://example.com/path*. Previously, the URL parser didn't support non-special URLs. The parser parses non-special URLs as if they had an opaque path, which is not aligned with the URL standard. Now, the URL parser parses non-special URLs correctly, following the URL standard. For more details, see [http://bit.ly/url-non-special](http://bit.ly/url-non-special).

### Policy updates

#### New policies

- [EdgeEntraCopilotPageContext](/deployedge/microsoft-edge-policies#edgeentracopilotpagecontext) - Control access to page content for Entra ID Profiles accessing Microsoft Copilot with Enterprise Data Protection (EDP) from the Microsoft Edge sidebar
- [ExtensionsPerformanceDetectorEnabled](/deployedge/microsoft-edge-policies#extensionsperformancedetectorenabled) - Extensions Performance Detector enabled

#### Deprecated policies

- [CopilotCDPPageContext](/deployedge/microsoft-edge-policies#copilotcdppagecontext) - Control Copilot with Commercial Data Protection access to page context for Microsoft Entra ID profiles (deprecated)

#### Obsoleted policies

- [AllowTokenBindingForUrls](/deployedge/microsoft-edge-policies#allowtokenbindingforurls) - Configure the list of sites for which Microsoft Edge will attempt to establish a Token Binding with (obsolete)


<!-- ===================== snip for archive ========================== -->
<!-- Version  129.0.2792.52: September 12, 2024 to Version 129.0.2792.89: October 10, 2024 --->
<!-- Version 128.0.2739.79: September 12, 2024 to Version 128.0.2739.42: August 22, 2024 --->
<!-- Version 127.0.2651.105: August 15, 2024 to Version 127.0.2651.74: July 25, 2024 --->
<!-- Version 126.0.2592.113: July 18, 2024 to Version 126.0.2592.61: June 17, 2024 --->
<!-- Version 124.0.2478.109: May 16, 2024 to Version 124.0.2478.51: April 18, 2024 -->
<!-- Version 123.0.2420.97: April 12, 2024 to Version 123.0.2420.53: March 22, 2024 -->
<!-- Version 122.0.2365.106: March 21, 2024 to Version 120.0.2210.181: February 20, 2024 -->
<!-- Version 121.0.2277.128: February 15, 2024 to Version 118.0.2088.122: November 29, 2023 -->
<!-- Version 119.0.2151.97: November 29, 2023 to Version 118.0.2088.57: October 18, 2023 -->
<!-- from Version 118.0.2088.46: October 13, 2023 to Version 109.0.1518.140: September 15, 2023 -->
<!-- from Version 117.0.2045.31: September 15, 2023 to Version 116.0.1938.62: August 25, 2023 -->
<!-- from Version 116.0.1938.54: August 21, 2023 to Version 114.0.1823.41: June 6, 2023 -->
<!-- from Version 114.0.1823.37: June 2, 2023 to Version 112.0.1722.77: May 9, 2023 -->
<!-- from Version 113.0.1774.35: May 5, 2023 to Version 112.0.1722.39: April 10, 2023 -->
<!-- from Version 112.0.1722.34: April 6, 2023 to Version 111.0.1661.43: March 15, 2023 -->
<!-- from Version 111.0.1661.41: March 13, 2023 to Version 110.0.1587.46: February 14, 2023 -->
<!-- from Version Version 110.0.1587.41: February 9, 2023 to Version 108.0.1462.83: January 12, 2023 -->
<!-- from Version 109.0.1518.49: January 12, 2023 to Version 108.0.1462.46: December 8, 2022 -->
<!-- from Version 108.0.1462.42: December 5, 2022 to Version 106.0.1370.59: October 27, 2022 -->
<!--- from Version 107.0.1418.24: October 27, 2022 to Version 106.0.1370.37: October 6, 2022 -->
<!--- from Version 106.0.1370.34: October 3, 2022 to Version 105.0.1343.27: September 2, 2022 -->
<!--- from Version 105.0.1343.25: September 1, 2022 to  Version 104.0.1293.70: August 25, 2022 -->
<!--- from Version 104.0.1293.63: August 19 to Version 102.0.1245.50: June 23 ---->
<!--- from Version 103.0.1264.37: June 23 to Version 102.0.1245.33: June 3 ---->
<!--- from Version 103.0.1264.37: June 23 to Version 102.0.1245.33: June 3 ---->
<!--- from Version 102.0.1245.30: May 31 to Version 100.0.1185.57: May 2 ---->
<!-- from Version 101.0.1210.32: April 28 to Version 100.0.1185.36: April 7 -->
<!---from Version 100.0.1185.29: April 1  to  Version 99.0.1150.36: March 7 --->
<!--- from Version 99.0.1150.30: March 3 to Version 98.0.1108.50: February 10 --->
<!--- from Version 98.0.1108.43: February 3 to Version 96.0.1054.72: January 6  -->
<!---- From Version 97.0.1072.55: January 6 to Version 96.0.1054.34: November 23 ---->
<!---archive from Version 96.0.1054.29: November 19 to Version 94.0.992.57: October 27 --->
<!-- archive from Version 95.0.1020.30: October 21 to Version 94.0.992.37: September 30 -->
<!-- archive from Version 94.0.992.31: September 24 to Version 93.0.961.44: September 9  -->
<!--- Archive from Version 93.0.961.38: September 2 to Version 92.0.902.62: July 29 --->
<!-- Archive from Version 92.0.902.55: July 22 to Version 91.0.864.37: May 27 -->
<!-- Archive from 89.0.774.45: March 4 to 90.0.818.66: May 20 ->
<!-- Archive from 86.0.622.43: October 15 to beta 88.0.705.81: February 25  ->
<!-- Archive from 86.0.622.38-october-9 to beta 86.0.62.215-september-14  ->
<!-- Archived to version 84.0.522.40: July 16 -->

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
