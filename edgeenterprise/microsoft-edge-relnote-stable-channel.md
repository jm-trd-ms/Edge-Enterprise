---
title: "Microsoft Edge release notes for Stable Channel"
ms.author: archandr
author: dan-wesley
manager: likuba
ms.date: 12/19/2024
audience: ITPro
ms.topic: conceptual
ms.service: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge release note for Stable Channel"
---

# Release notes for Microsoft Edge Stable Channel

These release notes provide information about new features and non-security updates that are included in the Microsoft Edge Stable Channel.

- All the security updates are listed in [Release notes for Microsoft Edge Security Updates](./microsoft-edge-relnotes-security.md).
- Archived release notes for Microsoft Edge Stable Channel are located in [Archived release notes for Microsoft Edge Stable Channel](./microsoft-edge-relnote-archive-stable-channel.md).

 To understand Microsoft Edge channels, see the [Overview of the Microsoft Edge channels](./microsoft-edge-channels.md).

> [!NOTE]
> For the Stable Channel, updates will roll out progressively over one or more days. To learn more, see [Progressive rollouts for Microsoft Edge updates](./microsoft-edge-update-progressive-rollout.md).
>
> Microsoft Edge Web Platform constantly evolves to improve user experience, security, and privacy. To learn more, see [Site compatibility-impacting changes coming to Microsoft Edge](/microsoft-edge/web-platform/site-impacting-changes).

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

Microsoft Edge WebView2 Runtime will no longer appear in the Installed Apps list in Windows Settings because it is a persistent system component.

### Dev Channel updates

The following Dev channel updates preceded this Stable channel release. The following Dev notes provide detailed information about the changes in each release.

- [Dev Channel update to 131.0.2863.0 is live. - Microsoft Community Hub](https://techcommunity.microsoft.com/discussions/edgeinsiderannouncements/dev-channel-update-to-131-0-2863-0-is-live-/4260359)
- [Dev Channel update to 131.0.2875.0 is live. - Microsoft Community Hub](https://techcommunity.microsoft.com/discussions/edgeinsiderannouncements/dev-channel-update-to-131-0-2875-0-is-live-/4267839)
- [Dev Channel update to 131.0.2889.0 is live. - Microsoft Community Hub](https://techcommunity.microsoft.com/discussions/edgeinsiderannouncements/dev-channel-update-to-131-0-2889-0-is-live-/4273465)
- [Dev Channel update to 131.0.2903.5 is live. - Microsoft Community Hub](https://techcommunity.microsoft.com/discussions/edgeinsiderannouncements/dev-channel-update-to-131-0-2903-5-is-live-/4277981)

### Feature updates

- **Cancel dialog for `beforeunload` event.** Microsoft Edge changed the behavior of the cancel dialog for the `beforeunload` event. Calling `event.preventDefault` in a `beforeunload` event handler won't prevent the dialog from being shown. Instead, `event.returnValue = ''` needs to be called in the `beforeunload` event handler to prevent the cancel dialog. The [BeforeunloadEventCancelByPreventDefaultEnabled](/deployedge/microsoft-edge-policies?branch=main#beforeunloadeventcancelbypreventdefaultenabled) policy is obsolete and no longer works after Microsoft Edge version 130.

- **Changes to Kyber.** The Kyber algorithm was standardized with minor technical changes and renamed to the Module Lattice Key Encapsulation Mechanism (ML-KEM). ML-KEM is implemented in the BoringSSL cryptography library, which allows for it to be deployed and utilized by services that depend on this library.

  The changes to the final version of ML-KEM make it incompatible with the previously deployed version of Kyber. Due to this incompatibility the following changes in Microsoft Edge will be made:

  - Edge switches from supporting Kyber to ML-KEM.
  - Edge offers a key share prediction for hybrid ML-KEM (codepoint 0x11EC).
  - The `PostQuantumKeyAgreementEnabled` flag and the [PostQuantumKeyAgreementEnabled](/deployedge/microsoft-edge-policies#postquantumkeyagreementenabled) policy applies to Kyber and ML-KEM. Note: The [PostQuantumKeyAgreementEnabled](/deployedge/microsoft-edge-policies#postquantumkeyagreementenabled) policy is scheduled for removal in Edge version 141.
  - Edge will no longer support hybrid Kyber (codepoint 0x6399).

- **New sidebar policy.** The [EdgeSidebarAppUrlHostAllowList](/deployedge/microsoft-edge-policies#edgesidebarappurlhostallowlist) policy allows admins to define a list of sites, based on URL patterns, that are not subject to the [EdgeSidebarAppUrlHostBlockList](/deployedge/microsoft-edge-policies#edgesidebarappurlhostblocklist). When the policy is configured, the apps listed in the allow list can be opened in sidebar even if they are listed in the block list. For more information, see [Manage the sidebar in Microsoft Edge](/deployedge/microsoft-edge-sidebar#allow-specific-sidebar-apps-except-search-using-urls).

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

## Version 129.0.2792.89: October 10, 2024

Fixed various bugs and performance issues.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#october-10-2024).

## Version 128.0.2739.113: October 10, 2024

Fixed various bugs and performance issues for Extended Stable channel.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#october-10-2024).

## Version 129.0.2792.79: October 3, 2024

Fixed various bugs and performance issues.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#october-3-2024).

## Version 128.0.2739.107: October 3, 2024

Fixed various bugs and performance issues for Extended Stable channel.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#october-3-2024).

## Version 128.0.2739.97: September 26, 2024

Fixed various bugs and performance issues for Extended Stable channel.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#september-26-2024).

## Version 129.0.2792.65: September 26, 2024

Fixed various bugs and performance issues, and feature updates.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#september-26-2024).

### Feature updates

- **Microsoft Edge sidebar updates.** For inactive sidebar users and new Edge users, the sidebar is turned OFF. Users can always return to **Settings > Sidebar** and turn the sidebar ON again at any time. For active sidebar users, the current sidebar state stays the same.
  
  Administrators can control the availability of the sidebar using the [HubsSidebarEnabled](/deployedge/microsoft-edge-policies#hubssidebarenabled) policy.

## Version 128.0.2739.90: September 19, 2024

Fixed various bugs and performance issues Extended Stable channel.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#september-19-2024).

## Version 129.0.2792.52: September 19, 2024

Fixed various bugs and performance issues, feature updates, site impacting compatibility changes, and policy updates.

Stable channel security updates are listed [here](/deployedge/microsoft-edge-relnotes-security#september-19-2024).

> [!NOTE]
> Portions of this release note are modifications based on work created and shared by Chromium.org and used according to terms described in the [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).

### Dev Channel updates

The following Dev channel updates preceded this Stable channel release. The following Dev notes provide detailed information about the changes in each release.

- [Dev Channel update to 129.0.2752.4 is live. - Microsoft Community Hub](https://techcommunity.microsoft.com/t5/articles/dev-channel-update-to-129-0-2752-4-is-live/m-p/4215208)
- [Dev Channel update to 129.0.2766.0 is live. - Microsoft Community Hub](https://techcommunity.microsoft.com/t5/articles/dev-channel-update-to-129-0-2766-0-is-live/m-p/4218361)
- [Dev Channel update to 129.0.2779.0 is live. - Microsoft Community Hub](https://techcommunity.microsoft.com/t5/articles/dev-channel-update-to-129-0-2779-0-is-live/m-p/4226574)
- [Dev Channel update to 129.0.2792.10 is live. - Microsoft Community Hub](https://techcommunity.microsoft.com/t5/articles/dev-channel-update-to-129-0-2792-10-is-live/m-p/4232423)

### Fixes

- **Policy updates to allow wildcards.** The documentation for the following policies were inaccurate and were corrected. These policies support wildcards (*) in URL patterns when being configured: [ImagesAllowedForUrls](/deployedge/microsoft-edge-policies#imagesallowedforurls), [ImagesBlockedForUrls](/deployedge/microsoft-edge-policies#imagesblockedforurls), [InsecureContentAllowedForUrls](/deployedge/microsoft-edge-policies#insecurecontentallowedforurls), [InsecureContentBlockedForUrls](/deployedge/microsoft-edge-policies#insecurecontentblockedforurls), [PopupsAllowedForUrls](/deployedge/microsoft-edge-policies#popupsallowedforurls), [PopupsBlockedForUrls](/deployedge/microsoft-edge-policies#popupsblockedforurls).

### Feature updates

- **Update to Microsoft Edge supported operating systems.** The minimum supported macOS version is increased to macOS 11. Users on older versions of macOS will no longer receive Microsoft Edge updates. For more information, see [Microsoft Edge Supported Operating Systems](/DeployEdge/microsoft-edge-supported-operating-systems).

- **Deprecation of the CryptoWallet feature.** To improve end user experience, the CryptoWallet feature and the [CryptoWalletEnabled](/deployedge/microsoft-edge-policies#cryptowalletenabled) policy is deprecated. The [CryptoWalletEnabled](/deployedge/microsoft-edge-policies#cryptowalletenabled) policy will be obsolete in an upcoming release.

### Site compatibility impacting changes

- **Deprecation of non-standard declarative shadow DOM serialization.** The prototype implementation, which shipped in 2020 and then updated in 2023, contained a method called `getInnerHTML()` that could be used to serialize DOM trees containing shadow roots. That part of the prototype wasn't standardized with the rest of the declarative shadow DOM, and has only recently reached spec consensus (for details, see [GitHub](https://github.com/whatwg/html/issues/8867). As part of that consensus, the shape of the `getInnerHTML` API changed.

- **Deprecate the includeShadowRoots argument on DOMParser.** The `includeShadowRoots` argument was a never-standardized argument to the `DOMParser.parseFromString()` function, which was there to allow imperative parsing of HTML content that contains declarative shadow DOM. This function was shipped as part of the initial shipment of declarative shadow DOM. Since the standards discussion rematerialized in 2023, the shape of DSD APIs changed, including this feature for imperative parsing.

  Now that a standardized version of this API, in the form of `setHTMLUnsafe()` and `parseHTMLUnsafe()` shipped, the non-standard `includeShadowRoots` argument needs to be deprecated and removed. All usage should shift accordingly:

  Instead of:

  `(new DOMParser()).parseFromString(html,'text/html',{includeShadowRoots: true});`

  This can be used instead:

  `document.parseHTMLUnsafe(html);`

- **Rename inset-area to position-area**. The CSS working group ([CSSWG](https://www.w3.org/groups/wg/css/)) resolved to rename this property from `inset-area` to `position-area`. For more information, see the CSSWG discussion in [GitHub](https://github.com/w3c/csswg-drafts/issues/10209#issuecomment-2221005001).

  The old and new property names are supported for a few milestones, to help developers migrate to the new position-area name. We're shipping the new property name, `position-area`, as a synonym for `inset-area`.

  The `inset-area` property is currently planned for removal in Microsoft Edge version 131.

### Policy updates

#### New policies

- [PrintingLPACSandboxEnabled](/deployedge/microsoft-edge-policies#printinglpacsandboxenabled) - Enable Printing LPAC Sandbox

#### Deprecated policies

- [CryptoWalletEnabled](/deployedge/microsoft-edge-policies#cryptowalletenabled) - Enable CryptoWallet feature (deprecated)
- [EnhanceSecurityModeOptOutUXEnabled](/deployedge/microsoft-edge-policies#enhancesecuritymodeoptoutuxenabled) - Manage opt-out user experience for Enhanced Security Mode (ESM) in Microsoft Edge (deprecated)

<!-- ===================== snip for archive ========================== -->
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
