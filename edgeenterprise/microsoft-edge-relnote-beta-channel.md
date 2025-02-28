---
title: "Microsoft Edge release notes for Beta Channel"
ms.author: archandr
author: dan-wesley
manager: likuba
ms.date: 02/10/2025
audience: ITPro
ms.topic: conceptual
ms.service: microsoft-edge
ms.localizationpriority: medium
ms.collection: M365-modern-desktop
description: "Microsoft Edge release notes for Beta Channel"
---

# Release notes for Microsoft Edge Beta Channel

These release notes provide information about new features and nonsecurity updates that are included in the Microsoft Edge Beta Channel. Archived versions of these release notes are available at [Archived release notes for Microsoft Edge Beta Channel](./microsoft-edge-relnote-archive-beta-channel.md).  

Get the latest Microsoft Edge for Business updates for your business, school, or organization at our [Download Page](https://www.microsoft.com/en-us/edge/business/download?form=MA13FQ)

> [!NOTE]
> Microsoft Edge Web Platform constantly evolves to improve user experience, security, and privacy. To learn more, see [Site compatibility-impacting changes coming to Microsoft Edge](/microsoft-edge/web-platform/site-impacting-changes).

## Version 134.0.3124.39: February 28, 2025

Fixed various bugs and performance issues. 

## Version 134.0.3124.31: February 24, 2025

Fixed various bugs and performance issues. 

## Version 134.0.3124.19: February 18, 2025

Fixed various bugs and performance issues. 

## Version 134.0.3124.8: February 13, 2025

Fixed various bugs and performance issues, Dev channel updates, feature updates, policy updates, and site compatibility impacting changes.

### Dev channel updates

The following Dev channel updates preceded this Beta channel release. These notes provide detailed information about the changes in each release.

- [Dev Channel update to 134.0.3081.2 is live. | Microsoft Community Hub](https://techcommunity.microsoft.com/discussions/edgeinsiderannouncements/dev-channel-update-to-134-0-3081-2-is-live-/4370518)
- [Dev Channel update to 134.0.3096.1 is live. | Microsoft Community Hub](https://techcommunity.microsoft.com/discussions/edgeinsiderannouncements/dev-channel-update-to-134-0-3096-1-is-live-/4372525)
- [Dev Channel update to 134.0.3109.0 is live. | Microsoft Community Hub](https://techcommunity.microsoft.com/discussions/edgeinsiderannouncements/dev-channel-update-to-134-0-3109-0-is-live-/4374330)
 
### Announcement

**Edge contextual capabilities in Business Chat work tab.**  Starting in mid to late March 2025, Microsoft Copilot in Edge will introduce support for page summarization and contextual queries to the Work tab for Microsoft 365 Copilot Business Chat. With this feature, users can ask Copilot contextual queries such as “summarize this page.” This feature will also include contextual prompt suggestions to help users ask relevant questions about open pages in Edge. Page summarization and contextual prompt suggestions are accessible for users when using Copilot through the Edge side pane.  
 
A Microsoft 365 Copilot license is required to use this feature.  Administrators can control the availability using the [EdgeEntraCopilotPageContext](/deployedge/microsoft-edge-policies#edgeentracopilotpagecontext) policy.  Broad availability of this feature will be announced via Microsoft Edge release notes.

### Feature updates

- **Removal of “Add account” option in Profile menu for Entra ID users.** The option to add a linked personal account directly from Edge is no longer available in the Edge profile menu.
 
- **Microsoft Search in Bing deprecation and policy updates.**  Microsoft Search in Bing, the work search experience available on Bing.com, will be retired, such that the last day of availability is on March 31, 2025. The [AddressBarMicrosoftSearchInBingProviderEnabled](/deployedge/microsoft-edge-policies#addressbarmicrosoftsearchinbingproviderenabled) policy, used to configure Microsoft Search in Bing results in the Edge for Business address bar, is deprecated in Microsoft Edge version 134 and will be obsoleted in a future Microsoft Edge version. The new policy to replace this is [AddressBarWorkSearchResultsEnabled](/deployedge/microsoft-edge-policies#addressbarworksearchresultsenabled) which is available in Microsoft Edge version 134. 

- **Edge Settings Improvements.**  Edge Settings is migrating to WebUI2 to boost page responsiveness and introducing a series of minor visual and content upgrades to improve overall usability and utility. This includes optimizing for concise wording of individual settings, simplifying the number of pages and reorganizing content, and creating a cohesive user interface. Note: This feature is a controlled feature rollout. If you don't see this feature, check back as we continue our rollout.

- **Scareware blocker policy.**  Scareware blocker in Microsoft Edge is your AI powered shield designed to protect you and your users from scareware attacks.  Scareware blocker is currently in preview and admins can control availability to this feature using the [ScarewareBlockerProtectionEnabled](/deployedge/microsoft-edge-policies#scarewareblockerprotectionenabled) Policy.  For more information, see [Stand up to scareware with scareware blocker, now available in preview in Microsoft Edge - Microsoft Edge Blog](https://blogs.windows.com/msedgedev/2025/01/27/stand-up-to-scareware-with-scareware-blocker/).

### Policy updates

#### New policies

- [AddressBarWorkSearchResultsEnabled](/deployedge/microsoft-edge-policies#addressbarworksearchresultsenabled) - Enable Work Search suggestions in the address bar
- [DefaultJavaScriptOptimizerSetting](/deployedge/microsoft-edge-policies#defaultjavascriptoptimizersetting) - Control use of JavaScript optimizers
- [IdleTimeout](/deployedge/microsoft-edge-policies#idletimeout) - Delay before running idle actions
- [IdleTimeoutActions](/deployedge/microsoft-edge-policies#idletimeoutactions) - Actions to run when the computer is idle
- [JavaScriptOptimizerAllowedForSites](/deployedge/microsoft-edge-policies#javascriptoptimizerallowedforsites) - Allow JavaScript optimization on these sites
- [JavaScriptOptimizerBlockedForSites](/deployedge/microsoft-edge-policies#javascriptoptimizerblockedforsites) - Block JavaScript optimizations on these sites
- [OopPrintDriversAllowed](/deployedge/microsoft-edge-policies#oopprintdriversallowed) - Out-of-process print drivers allowed
- [ScarewareBlockerProtectionEnabled](/deployedge/microsoft-edge-policies#scarewareblockerprotectionenabled) - Configure Edge Scareware Blocker Protection
- [ServiceWorkerToControlSrcdocIframeEnabled](/deployedge/microsoft-edge-policies#serviceworkertocontrolsrcdociframeenabled) - Allow ServiceWorker to control srcdoc iframes
- [SharedWorkerBlobURLFixEnabled](/deployedge/microsoft-edge-policies#sharedworkerbloburlfixenabled) - Make SharedWorker blob URL behavior aligned with the specification
- [WebAudioOutputBufferingEnabled](/deployedge/microsoft-edge-policies#webaudiooutputbufferingenabled) - Enable adaptive buffering for Web Audio

#### Obsoleted policies

- [UserAgentClientHintsGREASEUpdateEnabled](/deployedge/microsoft-edge-policies#useragentclienthintsgreaseupdateenabled) - Control the User-Agent Client Hints GREASE Update feature (obsolete)

>[!NOTE]
>For the latest web platform features and updates, see [Microsoft Edge 134 web platform release notes Mar. 2025](/microsoft-edge/web-platform/release-notes/134).

## Version 133.0.3065.59: February 10, 2025

Fixed various bugs and performance issues. 

## Version 133.0.3065.51: February 07, 2025

Fixed various bugs and performance issues. 

## Version 133.0.3065.49: February 05, 2025

Fixed various bugs and performance issues. 

## Version 133.0.3065.39: January 31, 2025

Fixed various bugs and performance issues. 

## Version 133.0.3065.31: January 27, 2025

Fixed various bugs and performance issues. 

## Version 133.0.3065.19: January 21, 2025

Fixed various bugs and performance issues. 

## Version 133.0.3065.10: January 17, 2025

Fixed various bugs and performance issues, Dev channel updates, feature updates, policy updates, and site compatibility impacting changes.

### Dev channel updates

The following Dev channel updates preceded this Beta channel release. These notes provide detailed information about the changes in each release.

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

- **Scareware blocker.** Scareware blocker in Microsoft Edge is your AI powered shield designed to protect you and your users from scareware attacks. Once enabled, scareware blocker uses machine learning (ML) to identify and block these scams, keeping you safe as you browse the web. For more information, [see Stand up to scareware with scareware blocker,](https://blogs.windows.com/msedgedev/2025/01/27/stand-up-to-scareware-with-scareware-blocker/) now available in preview in Microsoft Edge - Microsoft Edge Blog. **Note:** This experience is in preview and users can opt in via Microsoft Edge Settings, under `edge://settings/privacy`, Scareware is located under “Security”.  

- **Remove policy used for legacy same site behavior.** In Microsoft Edge version 80, we introduced the [LegacySameSiteCookieBehaviorEnabledForDomainList](/deployedge/microsoft-edge-policies#legacysamesitecookiebehaviorenabledfordomainlist) policy to revert the SameSite behavior of cookies to legacy behavior on the specified domains. The [LegacySameSiteCookieBehaviorEnabledForDomainList](/deployedge/microsoft-edge-policies#legacysamesitecookiebehaviorenabledfordomainlist) policy is obsolete in Microsoft Edge version 133.

- **Updated Downloads UI to Improve Performance.** The Downloads UI is rewritten to improve performance. Customer-facing functionality and UX from previous releases remain the same.

### Policy updates

#### New policies
- [CACertificateManagementAllowed](/deployedge/microsoft-edge-policies#cacertificatemanagementallowed) - Allow users to manage installed CA certificates
- [CA Certificates](/deployedge/microsoft-edge-policies#cacertificates) - TLS server certificates that should be trusted by Microsoft Edge
- [CACertificatesWithConstraints](/deployedge/microsoft-edge-policies#cacertificateswithconstraints) - TLS certificates that should be trusted by Microsoft Edge for server authentication with constraints
- [CADistrustedCertificates](/deployedge/microsoft-edge-policies#cadistrustedcertificates) - TLS certificates that should be distrusted by Microsoft Edge for server authentication
- [CAHintCertificates](/deployedge/microsoft-edge-policies#cahintcertificates) - TLS certificates that are not trusted or distrusted but can be used in path-building for server authentication
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

### Site compatibility impacting changes

> [!NOTE]
> Portions of this release note are modifications based on work created and shared by Chromium.org and used according to terms described in the [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).

- **CSS advanced attr() function.** Implements the augmentation to `attr()` specified in CSS Level 5, which allows types besides `<string>` and use in all CSS properties (in addition to the existing support for the pseudo-element `content`).

- **CSS `:open` pseudo-class.** The `:open` pseudo-class matches `<dialog>` and `<details>` when they are in their open state, and matches `<select>` and `<input>` when they are in modes which have a picker and the picker is showing.

- **CSS scroll state container queries.** Use container queries to style descendants of containers based on their scroll state.

    The query container is either a scroll container, or an element affected by the scrolled position of a scroll container. The following states can be queried:
    - `stuck`: A sticky positioned container is stuck to one of the edges of the scroll box.
    - `snapped`: A scroll snap aligned container is currently snapped horizontally or vertically.
    - `scrollable`: Whether a scroll container can be scrolled in a queried direction.

    A new `container-type: scroll-state` lets containers be queried.

    ```css
    #sticky {
      position: sticky;
      container-type: scroll-state;
    }

    @container scroll-state(stuck: top) {
      #sticky-child {
        font-size: 75%;
      }
    }
    ```
- **CSS `text-box`, `text-box-trim`, and `text-box-edge`.** To achieve optimal balance of text content, the `text-box-trim` and `text-box-edge` properties, along with the `text-box` shorthand property, make finer control of vertical alignment of text possible.

    The `text-box-trim` property specifies the sides to trim, above or below, and the `text-box-edge` property specifies how the edge should be trimmed.

    These properties let you control vertical spacing precisely by using the font metrics.

- **The `hint` value of the `popover` attribute.**  The Pop over API specifies the behavior for two values of the `popover` attribute: `auto` and `manual`. This feature describes a third value, `popover=hint`. Hints, which are most often associated with "tooltip" type behaviors, have slightly different behaviors. Primarily, the difference is that a `hint` is subordinate to auto when opening nested stacks of popovers. So it's possible to open an unrelated `hint` popover while an existing stack of `auto` popovers stays open.

    The canonical example is that a `<select>` picker is open (`popover=auto`) and a hover-triggered tooltip (`popover=hint`) is shown. That action doesn't close the `<select>` picker.

- **Popover invoker and anchor positioning improvements.** Adds an imperative way to set invoker relationships between popovers with `popover.showPopover({source})`. Enables invoker relationships to create implicit anchor element references.

- **Popover nested inside invoker shouldn't re-invoke it.** In the following case clicking the button properly activates the popover, however, clicking on the popover itself after that shouldn't close the popover.

  ```css
  <button popovertarget=foo>Activate
    <div popover id=foo>Clicking me shouldn't close me</div>
  </button>
  ```

  Previously this happened, because the popover select bubbles to the `<button>` and activates the invoker, which toggles the popover closed. This has now been changed to the expected behavior.

- **`Animation.overallProgress`.** Provides developers with a convenient and consistent representation of how far along an animation has advanced across its iterations and regardless of the nature of its timeline. Without the `overallProgress` property, you need to manually compute how far an animation has advanced, factoring in the number of iterations of the animation and whether the `currentTime` of the animation is a percentage of total time (as in the case of scroll-driven animations) or an absolute time quantity (as in the case of time-driven animations).

- **The `pause()` method of the `Atomics` object.** Adds the `pause()` method to the `Atomics` namespace object, to hint the CPU that the current code is executing a spinlock.

- **CSP hash reporting for scripts.**  Complex web applications often need to keep track of the subresources that they download, for security purposes.

    In particular, upcoming industry standards and best practices (for example, PCI-DSS v4) require that web applications keep an inventory of all the scripts they download and execute.

    This feature builds on CSP and the Reporting API to report the URLs and hashes (for CORS/same-origin) of all the script resources that the document loads.

- **DOM state-preserving move.** Adds a DOM primitive (`Node.prototype.moveBefore`) that lets you move elements around a DOM tree, without resetting the element's state.

    When moving instead of removing and inserting, state such as the following is preserved:
    - `<iframe>` elements remain loaded.
    - The active element remains focus.
    - Popovers, fullscreen, and modal dialogs remain open.
    - CSS transitions and animations continue.

- **Expose `attributionsrc` attribute on `<area>`.**  Aligns exposure of the `attributionsrc` attribute on `<area>` with the existing processing behavior of the attribute, even when it wasn't exposed.

    Additionally, it makes sense to support the attribute on `<area>`, as that element is a first-class navigation surface, and Microsoft Edge already supports this on the other surfaces of `<a>` and `window.open`

- **Expose coarsened cross-origin `renderTime` in element timing and LCP (regardless of `Timing-Allow-Origin`).** Element timing and LCP entries have a `renderTime` attribute, aligned with the first frame in which an image or text was painted.

    This attribute is currently guarded for cross-origin images by requiring a `Timing-Allow-Origin` header on the image resource. However, that restriction is easy to work around (for example, by displaying a same-origin and cross-origin image in the same frame).

    Since this has been a source of confusion, we instead plan to remove this restriction, and instead coarsen all render times by 4 ms when the document isn't cross-origin-isolated. This is seemingly coarse enough to avoid leaking any useful decoding-time information about cross-origin images.

- **The `FileSystemObserver` interface.** The `FileSystemObserver` interface notifies websites of changes to the file system. Sites observe changes to files and directories, to which the user has previously granted permission, in the user's local device, or in the Bucket File System (also known as the Origin Private File System), and are notified of basic change info, such as the change type.

- **Multiple import maps.** Import maps currently have to load before any ES module and there can only be a single import map per document. That makes them fragile and potentially slow to use in real-life scenarios: Any module that loads before them breaks the entire app, and in apps with many modules they become a large blocking resource, as the entire map for all possible modules needs to load first.

    This feature enables multiple import maps per document, by merging them in a consistent and deterministic way.

- **Storage Access Headers.**  Offers an alternate way for authenticated embeds to opt in for unpartitioned cookies. These headers indicate whether unpartitioned cookies are (or can be) included in a given network request, and allow servers to activate `storage-access` permissions they have already been granted. Giving an alternative way to activate the `storage-access` permission allows usage by noniframe resources, and can reduce latency for authenticated embeds.

- **Support creating `ClipboardItem` with `Promise<DOMString>.`**  The `ClipboardItem`, which is the input to the async clipboard `write()` method, now accepts string values in addition to Blobs in its constructor. `ClipboardItemData` can be a Blob, a string, or a Promise that resolves to either a Blob or a string.

- **WebAssembly Memory64.** The [memory64 proposal](https://github.com/WebAssembly/memory64/blob/main/proposals/memory64/Overview.md) adds support for linear WebAssembly memories with size larger than 2^32 bits. It provides no new instructions, but instead extends the existing instructions to allow 64-bit indexes for memories and tables.

- **Web Authentication API: PublicKeyCredential `getClientCapabilities()` method.** The PublicKeyCredential `getClientCapabilities()` method lets you determine which WebAuthn features are supported by the user's client. The method returns a list of supported capabilities, allowing developers to tailor authentication experiences and workflows based on the client's specific functionality.

- **WebGPU: 1-component vertex formats (and unorm8x4-bgra).**  Adds additional vertex formats not present in the initial release of WebGPU due to lack of support or old macOS versions (which are no longer supported by any browser). The 1-component vertex formats let applications request only the necessary data when previously they had to request at least two times more for 8-bit and 16-bit data types. The unorm8x4-bgra format makes it slightly more convenient to load BGRA-encoded vertex colors while keeping the same shader.

- **X25519 algorithm of the Web Cryptography API.**  The "X25519" algorithm provides tools to perform key agreement using the X25519 function specified in [RFC7748]. The "X25519" algorithm identifier can be used in the SubtleCrypto interface to access the implemented operations: generateKey, importKey, exportKey, deriveKey, and deriveBits.

- **Deprecate the WebGPU `maxInterStageShaderComponents` limit.**  The `maxInterStageShaderComponents limit` is deprecated due to a combination of factors. The intended removal date in Microsoft Edge 135.
    - Redundancy with `maxInterStageShaderVariables`: This limit already serves a similar purpose, controlling the amount of data passed between shader stages.
    - Minor discrepancies: While there are slight differences in how the two limits are calculated, these differences are minor and can be effectively managed within the `maxInterStageShaderVariables` limit.
    - Simplification: Removing `maxInterStageShaderComponents` streamlines the shader interface and reduces complexity for developers. Instead of managing two separate limits with subtle differences, they can focus on the more appropriately named and comprehensive `maxInterStageShaderVariables`.

- **Remove `<link rel=prefetch>` five-minute rule.**  Previously, when a resource was prefetched using `<link rel=prefetch>`, Microsoft Edge ignored its cache semantics (namely `max-age` and `no-cache`) for the first use within five minutes, to avoid refetching. Now, Microsoft Edge removes this special case and uses normal HTTP cache semantics.

    This means web developers need to include appropriate caching headers (Cache-Control or Expires) to see benefits from `<link rel=prefetch>`.

    This also affects the nonstandard `<link rel=prerender>`.


## Version 132.0.2957.111: January 15, 2025

Fixed various bugs and performance issues. 

## Version 132.0.2957.106: January 13, 2025

Fixed various bugs and performance issues. 

## Version 132.0.2957.101: January 11, 2025

Fixed various bugs and performance issues.

## Version 132.0.2957.93: January 6, 2025

Fixed various bugs and performance issues.

## Version 132.0.2957.55: December 16, 2024

Fixed various bugs and performance issues.

## Version 132.0.2957.41: December 9, 2024

Fixed various bugs and performance issues.

## Version 132.0.2957.26: December 2, 2024

Fixed various bugs and performance issues, and feature updates.

### Feature updates

- **Deprecation of Microsoft Edge Support page.** To improve end user experience, *edge://support* is being deprecated. The information found on *edge://support* is available on other pages: *edge://version*, *edge://metrics-internals*, *edge://extensions*, and *edge://policy*.

- **AI theme generator.** Microsoft Edge includes an AI theme generator that allows users to input a text string and generate a series of images to preview as browser themes. Applying the theme includes setting the generated image on the Microsoft Edge new tab page and applying the image's dominant color to the browser frame.  Users can now find a new entry point in *edge://settings/appearance* which directs them to [AI Theme Generator: Create a Custom Browser Theme](https://www.microsoft.com/en-us/edge/create-a-theme?ep=762&es=147&form=MT00OT). Admins can control availability to this feature using the [AIGenThemesEnabled](/deployedge/microsoft-edge-policies#aigenthemesenabled) policy. If an admin chooses to disable the feature via policy, the page linked in Microsoft Edge Settings is available, but users will not be allowed to generate images and they see an error message. **Note:** This is a controlled feature rollout. If you don't see this feature, check back as we continue our rollout.

## Version 132.0.2957.11: November 22, 2024

Fixed various bugs and performance issues, Dev channel updates, feature updates, policy updates, and site compatibility impacting changes.

### Dev channel updates

The following Dev channel updates preceded this Beta channel release. These notes provide detailed information about the changes in each release.

- [Dev Channel update to 132.0.2917.0 is live. | Microsoft Community Hub](https://techcommunity.microsoft.com/discussions/edgeinsiderannouncements/dev-channel-update-to-132-0-2917-0-is-live-/4283359)
- [Dev Channel update to 132.0.2931.1 is live. | Microsoft Community Hub](https://techcommunity.microsoft.com/discussions/edgeinsiderannouncements/dev-channel-update-to-132-0-2931-1-is-live-/4288628)
- [Dev Channel update to 132.0.2945.0 is live. | Microsoft Community Hub](https://techcommunity.microsoft.com/discussions/edgeinsiderannouncements/dev-channel-update-to-132-0-2945-0-is-live-/4296080)

### Feature updates

- **Intune policies in the Microsoft Edge management service.** Admins now can set Intune policies via the Microsoft Edge management service, alongside the existing cloud policies. This ability lets admins deploy both browser policies in the cloud and Intune policies from a single pane, making it easy to keep users safe and the browser workflow streamlined. This feature comes along with a new policy creation wizard that streamlines the creation process into a comprehensive, step-by-step flow. **Note:** This experience is in public preview and can be accessed by opting in to targeted release in the Microsoft 365 admin center.

- **Version monitoring in the Edge management service.** The Edge management service offers a single view of all managed Microsoft Edge instances with their update status and possible actions to take. For out-of-date devices, you can easily schedule updates or notify users to update their browsers to avoid workflow interruptions. **Note:** This experience is in public preview and can be accessed by opting in to targeted release in the Microsoft 365 admin center.

- **Shopping Product Tracking.** Track product prices easily with a new experience in the Microsoft Edge Address Bar that appears on the product detail page. Users can track prices quickly and are notified when there's a price drop on that product and save more. Administrators can control the availability of Shopping in Microsoft Edge using the [EdgeShoppingAssistantEnabled](/deployedge/microsoft-edge-policies#edgeshoppingassistantenabled) policy. **Note:** This feature is a controlled feature rollout. If you don't see this feature, check back as we continue our rollout.

- **Feature Usage Data Sync.** Microsoft Edge Sync, which enables users to synchronize their Microsoft Edge user data across multiple devices, is now launching a new sync data category called Feature Usage. This new category allows users to synchronize data regarding their utilization of Microsoft Edge features across all their devices. **Note:** This feature is a controlled feature rollout. If you don't see this feature, check back as we continue our rollout.

- **New password manager policy.** The [DeletingUndecryptablePasswordsEnabled](/deployedge/microsoft-edge-policies#deletingundecryptablepasswordsenabled) policy controls whether the built-in password manager can delete undecryptable passwords from its database. This policy is required to restore the full functionality of the built-in password manager, but it might cause permanent data loss. Undecryptable password values won't become decryptable on their own. If fixing them is possible, it usually requires complex user actions.

- **PromotionalTabsEnabled policy deprecation.** The [PromotionalTabsEnabled](/deployedge/microsoft-edge-policies#promotionaltabsenabled) policy is deprecated in Microsoft Edge version 132 and will be obsolete in a future Microsoft Edge version. Administrators can use the [ShowRecommendationsEnabled](/deployedge/microsoft-edge-policies#showrecommendationsenabled) policy instead.

- **Allow enterprise users to view XFA PDFs using IE Mode.** Enterprise customers can view XFA PDFs in Microsoft Edge using IE mode through either the [ViewXFAPDFInIEModeAllowedOrigins](/deployedge/microsoft-edge-policies#viewxfapdfiniemodeallowedorigins) or [ViewXFAPDFInIEModeAllowedFileHash](/deployedge/microsoft-edge-policies#viewxfapdfiniemodeallowedfilehash) policy. This change is available in the new PDF viewer on Microsoft Edge.

### Policy updates

#### New policies

- [AdHocCodeSigningForPWAsEnabled](/deployedge/microsoft-edge-policies#adhoccodesigningforpwasenabled) - Native application signing during Progressive Web Application installation
- [AutomaticFullscreenAllowedForUrls](/deployedge/microsoft-edge-policies#automaticfullscreenallowedforurls) - Allow automatic full screen on specified sites
- [AutomaticFullscreenBlockedForUrls](/deployedge/microsoft-edge-policies#automaticfullscreenblockedforurls) - Block automatic full screen on specified sites
- [CreatePasskeysInICloudKeychain](/deployedge/microsoft-edge-policies#createpasskeysinicloudkeychain) - Control whether passkey creation defaults to iCloud Keychain
- [DeletingUndecryptablePasswordsEnabled](/deployedge/microsoft-edge-policies#deletingundecryptablepasswordsenabled) - Enable deleting undecryptable passwords
- [GenAILocalFoundationalModelSettings](/deployedge/microsoft-edge-policies#genailocalfoundationalmodelsettings) - Settings for GenAI local foundational model
- [IPv6ReachabilityOverrideEnabled](/deployedge/microsoft-edge-policies#ipv6reachabilityoverrideenabled) - Enable IPv6 reachability check override
- [LiveTranslationAllowed](/deployedge/microsoft-edge-policies#livetranslationallowed) - Live translation allowed
- [PersonalizeTopSitesInCustomizeSidebarEnabled](/deployedge/microsoft-edge-policies#personalizetopsitesincustomizesidebarenabled) - Personalize my top sites in Customize Sidebar enabled by default

- [ViewXFAPDFInIEModeAllowedFileHash](/deployedge/microsoft-edge-policies#viewxfapdfiniemodeallowedfilehash)- View XFA-based PDF files using IE Mode for allowed file hash.
- [ViewXFAPDFInIEModeAllowedOrigins](/deployedge/microsoft-edge-policies#viewxfapdfiniemodeallowedorigins) - View XFA-based PDF files using IE Mode for allowed file origin.
- [SelectParserRelaxationEnabled](/deployedge/microsoft-edge-policies#selectparserrelaxationenabled) - Controls whether the new HTML parser behavior for the `<select>` element is enabled

#### Deprecated policies

- [InsecureFormsWarningsEnabled](/deployedge/microsoft-edge-policies#insecureformswarningsenabled) - Enable warnings for insecure forms (deprecated)
- [MutationEventsEnabled](/deployedge/microsoft-edge-policies#mutationeventsenabled) - Enable deprecated/removed Mutation Events (deprecated)
- [PromotionalTabsEnabled](/deployedge/microsoft-edge-policies#promotionaltabsenabled)- Enable full-tab promotional content (deprecated)

#### Obsoleted policies

- [BlockTruncatedCookies](/deployedge/microsoft-edge-policies#blocktruncatedcookies) - Block truncated cookies (obsolete)
- [CertificateTransparencyEnforcementDisabledForLegacyCas](/deployedge/microsoft-edge-policies#certificatetransparencyenforcementdisabledforlegacycas) - Disable Certificate Transparency enforcement for a list of legacy certificate authorities (obsolete)

### Site compatibility impacting changes

> [!NOTE]
> Portions of this release note are modifications based on work created and shared by Chromium.org and used according to terms described in the [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).

- **CSS Anchor Positioning: allow `anchor-size()` in inset and margin properties.** Originally, `anchor-size()` was only allowed in sizing properties. The specification now allows `anchor-size()` in insets and margins as well.

- **CSS sideways writing modes.** Support of `sideways-rl` and `sideways-lr` keywords for the `writing-mode` CSS property. `sideways-rl` and `sideways-lr` are helpful to write non-CJK text vertically. They don't have behaviors favorable for CJK languages unlike `vertical-rl` and `vertical-lr`.

- **Dialog toggle events.** This change incorporates the same `ToggleEvent` that popovers dispatch, but for `<dialog>` elements: when `showModal` or `show` is called, `<dialog>` dispatches a `ToggleEvent` with `newState=open`. When a `<dialog>` is closed (using the form, button, or close watcher) it should dispatch a `ToggleEvent` with `newState=closed`.

  Previously, to detect when a `<dialog>` opens a mutation observer had to be registered to check for open.

- **Element Capture.** Given a video `MediaStreamTrack` obtained through preexisting means to initiate tab-capture, Element Capture allows mutating the track to only capture a subtree of the DOM starting at a given Element.

  The API bears some resemblance to the Region Capture API, but affords greater flexibility for applications, because occluding and occluded content are both excluded from the capture.

- **FedCM authorization features.** This bundles a few features that Identity Providers (IdP) can use to implement authorization flows such as letting a user grant access to their calendar to a Relying Party (RP). Specifically:

  - The IdP needs to be able to show a custom prompt for the permission (continuation API).
  - The RP needs an extensible way to communicate to the IdP what it wants access to (parameters API).
  - The RP needs to be able to customize or suppress the text referring to the IdP sharing "name, email address, and profile picture" because in this situation they're asking for different information (fields API).
  - The IdP might want to use a different endpoint to implement the authorization flow (multiple configURLs).
  - Certain accounts may only be eligible for one of the authentication and authorization flows and so there needs to be a way to show different accounts in the two flows (account labels API).

- **FedCM Mode API and Use Other Account API.** Two new extensions for FedCM:

  - **Mode**: The `active` mode allows websites to call FedCM inside a button select (for example, selecting a **Sign-in to IdP** button), which requires FedCM to guarantee it always responds with a visible user interface. Calling the FedCM API in *active mode* takes users to sign in to the Identity Provider (IdP) when users are logged-out. Also, because the active mode is called within an explicit user gesture, the UI is also more prominent (for example, centered and modal) compared to the UI from the passive mode (which doesn't require a user gesture requirement and can be called on page load).
  - **Use Other Account**: With this extension, an IdP can allow users to sign in to other accounts.

- **Fetch: `Request.bytes()` and `Response.bytes()`.** Add a `bytes()` method to the `Request` and `Response` interfaces, which returns a promise that resolves with a Uint8Array. While `Request` and `Response` have an `arrayBuffer()` method, it’s not possible to read directly from a buffer. A view such as a `Uint8Array` must be created to read it. The `bytes()` method improves the ergonomics of getting the body of Request and Response.

- **Ignore Strict-Transport-Security for localhost.** `Strict-Transport-Security` (STS) response headers can cause problems for localhost web servers because STS applies host-wide, across all ports. This causes compatibility problems for web developers testing locally. It also affects end-users who use software packages that commonly start localhost web servers for ephemeral reasons. For example, communication of an auth token from a web sign-in to a local software package. If one local listener sets `Strict-Transport-Security` on a localhost response, it's applied to all subsequent localhost requests regardless of port.

  Microsoft Edge 132 resolves this problem by ignoring `Strict-Transport-Security` headers on responses from localhost URLs.
  
- **Keyboard focusable scroll containers.** The rollout of this feature (from Microsoft Edge 130) was stopped due to an accessibility regression. This issue is fixed and the feature continues to roll out with Microsoft Edge 132. [KeyboardFocusableScrollersEnabled]( /deployedge/microsoft-edge-policies#keyboardfocusablescrollersenabled) is the policy for this feature.

- **Private State Token API Permissions Policy default allowlist wildcard.** Access to the Private State Token API is gated by Permissions Policy features. Microsoft Edge 132 updates the default allowlist for both `private-state-token-issuance` and `private-state-token-redemption` features from `self` to `*` (wildcard).

- **`PushMessageData::bytes()`.** The `PushMessageData` interface mimics the `Body` interface, which was amended earlier this year with a new `bytes()` method, following the principle that APIs should generally vend byte buffers as `Uint8Arrays`. Microsoft Edge 132 realigns with the `Body` interface by providing the `bytes()` accessor on the `PushMessageData` interface as well.

- **Saved queries in `sharedStorage.selectURL`.** `sharedStorage.selectURL()` now lets queries to be saved and reused on a per-page basis. Two per-page-load budgets are charged the first time a saved query is run but not for subsequent runs of the saved query during the same page-load. This change is accomplished with a `savedQuery` parameter in the options for `selectURL()` that names the query.

- **Throw exception for popovers and dialogs in non-active documents.** Previously calling `showPopover()` or `showModal()` on a popover or dialog that resides within an inactive document would silently fail. No exception was thrown, but since the document is inactive, no popover or dialog would be shown. As of Microsoft Edge 132, these situations now throw `InvalidStateError`.

- **WebAuthn Signal API.** Allows WebAuthn relying parties to signal information about existing credentials back to credential storage providers, so that incorrect or revoked credentials can be updated or removed from provider and system UI.

- **WebGPU: 32-bit float textures blending.** The `float32-blendable` GPU feature makes GPU textures with formats `r32float`, `rg32float`, and `rgba32float` blendable.

- **WebGPU: Expose GPUAdapterInfo from GPUDevice.** The GPUDevice `adapterInfo` attribute exposes the same `GPUAdapterInfo` as the `GPUAdapter` object.

- **WebGPU: Texture view usage.** Adds an optional field to WebGPU texture view creation to request a subset of the usage flags from the source texture.

  By default, texture view usage inherits from the source texture but there are view formats that can be incompatible with the full set of inherited usages. Adding a usage field to texture view creation allows the user request a subset of the source texture's usages that are valid with the view format and specific to their intended usage of the texture view.

  WebGPU implementations can also optimize the creation of low level resources and improve performance when using views with more specialized usage flags.

- **New origin trials: Document-Isolation-Policy.** The **Document-Isolation-Policy** lets a document enable `crossOriginIsolation` for itself, without having to deploy COOP or COEP, and regardless of the `crossOriginIsolation` status of the page. The policy is backed by process isolation. Additionally, the document non-CORS cross-origin subresources will either be loaded without credentials or will need to have a CORP header.

- **New origin trials: Explicit Compile Hints with Magic Comments.** This feature lets you attach information about which functions should be eager parsed and compiled in JavaScript files. The information is encoded as magic comments.

- **`navigator.storage` no longer an EventTarget.** `navigator.storage` was made an `EventTarget` for the Storage Pressure Event, which never made it past the prototype phase. This dead code is being removed and as a result, `navigator.storage` will no longer extend `EventTarget`.

- **Remove Prefixed HTMLVideoElement Fullscreen APIs.** The prefixed HTMLVideoElement fullscreen APIs have been deprecated from Microsoft Edge.

  They were replaced by the `Element.requestFullscreen()` API. As of 2024, most browsers have had support for the unprefixed APIs for a few years now.

  Microsoft Edge 132 removes the following from `HTMLVideoElement`:

  - The `webkitSupportsFullscreen` attribute.
  - The `webkitDisplayingFullscreen` attribute.
  - The `webkitEnterFullscreen()` method.
  - The `webkitExitFullscreen()` method. Note the different capitalization of the "S" in FullScreen.
  - The `webkitEnterFullScreen()` method.
  - The `webkitExitFullScreen()` method.

  These methods are now only aliases for the modern API. Their use has declined steadily over the years.

  ## Version 131.0.2903.51: November 15, 2024

Fixed various bugs and performance issues.

## Version 131.0.2903.48: November 14, 2024

Fixed various bugs and performance issues.

## Version 131.0.2903.45: November 13, 2024

Fixed various bugs and performance issues.

## Version 131.0.2903.36: November 8, 2024

Fixed various bugs and performance issues, and feature updates.

> [!NOTE]
> Portions of this release note are modifications based on work created and shared by Chromium.org and used according to terms described in the [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).

### Feature updates

- **Changes to Kyber.** The Kyber algorithm was standardized with minor technical changes and renamed to the Module Lattice Key Encapsulation Mechanism (ML-KEM). ML-KEM is implemented in the BoringSSL cryptography library, which allows for it to be deployed and utilized by services that depend on this library.

  The changes to the final version of ML-KEM make it incompatible with the previously deployed version of Kyber. Due to this incompatibility the following changes in Microsoft Edge will be made:

  - Microsoft Edge switches from supporting Kyber to ML-KEM.
  - Microsoft Edge offers a key share prediction for hybrid ML-KEM (codepoint 0x11EC).
  - The `PostQuantumKeyAgreementEnabled` flag and the [PostQuantumKeyAgreementEnabled](/deployedge/microsoft-edge-policies#postquantumkeyagreementenabled) policy applies to Kyber and ML-KEM.
  - Microsoft Edge will no longer support hybrid Kyber (codepoint 0x6399).

## Version 131.0.2903.27: November 4, 2024

Fixed various bugs and performance issues.

## Version 131.0.2903.14: October 28, 2024

Fixed various bugs and performance issues.

## Version 131.0.2903.9: October 24, 2024

Fixed various bugs and performance issues, Dev channel updates, feature updates, site compatibility impacting changes, and policy updates.

> [!NOTE]
> Portions of this release note are modifications based on work created and shared by Chromium.org and used according to terms described in the [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).

### Dev Channel updates

The following Dev channel updates preceded this Beta channel release. These notes provide detailed information about the changes in each release.

- [Dev Channel update to 131.0.2863.0 is live. - Microsoft Community Hub](https://techcommunity.microsoft.com/t5/articles/dev-channel-update-to-131-0-2863-0-is-live/m-p/4260359)
- [Dev Channel update to 131.0.2875.0 is live. - Microsoft Community Hub](https://techcommunity.microsoft.com/t5/articles/dev-channel-update-to-131-0-2875-0-is-live/m-p/4267839)
- [Dev Channel update to 131.0.2889.0 is live. - Microsoft Community Hub](https://techcommunity.microsoft.com/t5/articles/dev-channel-update-to-131-0-2889-0-is-live/m-p/4273465)
- [Dev Channel update to 131.0.2903.5 is live. - Microsoft Community Hub](https://techcommunity.microsoft.com/t5/articles/dev-channel-update-to-131-0-2903-5-is-live/m-p/4277981)

### Feature updates

- **Cancel dialog for `beforeunload` event.** Microsoft Edge changed the behavior of the canceled dialog for the `beforeunload` event. Calling `event.preventDefault` in a `beforeunload` event handler won't prevent the dialog from being shown. Instead, `event.returnValue = ''` needs to be called in the `beforeunload` event handler to prevent the canceled dialog. The [BeforeunloadEventCancelByPreventDefaultEnabled](/deployedge/microsoft-edge-policies?branch=pr-en-us-4908#beforeunloadeventcancelbypreventdefaultenabled) policy is obsolete and no longer works after Microsoft Edge version 130.

- **Get the latest updates effortlessly with instant update.** Instant update in Microsoft Edge ensures you get the latest browser updates automatically, when you step away from your computer. You can keep browsing, knowing that you already have the latest updates to keep you safe online. For more information, see [Get instant updates in Microsoft Edge - Microsoft Support](https://support.microsoft.com/microsoft-edge/get-instant-updates-in-microsoft-edge-4820adad-dd32-470c-9bd9-dba1de71a7f1). **Note:** This feature is in private preview for enterprise customers. Future feature updates are available via Microsoft Edge release notes.

### Site compatibility impacting changes

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

- **Remove non-standard GPUAdapter `requestAdapterInfo()` method.** The WebGPU Working Group decided it was impractical for `requestAdapterInfo()` to trigger a permission prompt so they've removed that option and replaced it with the GPU Adapter `info` attribute so that web developers can get the same `GPUAdapterInfo` value synchronously.

### Policy updates

#### New policies

- [EdgeSidebarAppUrlHostAllowList](/deployedge/microsoft-edge-policies#edgesidebarappurlhostallowlist) - Allow specific apps to be opened in Microsoft Edge sidebar
- [PrivateNetworkAccessRestrictionsEnabled](/deployedge/microsoft-edge-policies#privatenetworkaccessrestrictionsenabled) - Specifies whether to apply restrictions to requests to more private network endpoints

#### Deprecated policies

- [NewBaseUrlInheritanceBehaviorAllowed](/deployedge/microsoft-edge-policies#newbaseurlinheritancebehaviorallowed) - Allows enabling the feature NewBaseUrlInheritanceBehavior (deprecated)
- [RSAKeyUsageForLocalAnchorsEnabled](/deployedge/microsoft-edge-policies#rsakeyusageforlocalanchorsenabled) - Check RSA key usage for server certificates issued by local trust anchors (deprecated)
- [UserAgentClientHintsGREASEUpdateEnabled](/deployedge/microsoft-edge-policies#useragentclienthintsgreaseupdateenabled) - Control the User-Agent Client Hints GREASE Update feature (deprecated)

#### Obsoleted policies

- [BeforeunloadEventCancelByPreventDefaultEnabled](/deployedge/microsoft-edge-policies#beforeunloadeventcancelbypreventdefaultenabled) - Control the behavior for the canceled dialog produced by the before unload event (obsolete)
- [SignInCtaOnNtpEnabled](/deployedge/microsoft-edge-policies#signinctaonntpenabled) - Enable sign in select to action dialog (obsolete)



<!--=========================== archived =================================-->
<!--Version 130.0.2849.52: October 23, 2024 to Version 130.0.2849.5: September 26, 2024 -->
<!-- Version 129.0.2792.52: September 19, 2024 to Version 129.0.2792.12: August 29, 2024 -->
<!-- Version 128.0.2739.42: August 22, 2024 to Version 128.0.2739.5: August 1, 2024 -->
<!-- Version 127.0.2651.74: July 25, 2024 to Version 127.0.2651.8: June 21, 2024 -->
<!-- Version 126.0.2592.68: June 20, 2024 to Version 126.0.2592.13: May 23, 2024 -->
<!-- Version 125.0.2535.51: May 17, 2024 to Version 125.0.2535.13: April 29, 2024 -->
<!-- Version 124.0.2478.67: April 26, 2024 to Version 124.0.2478.10: March 28, 2024 -->
<!-- Version 123.0.2420.65: March 27, 2024 to Version 122.0.2365.8: February 1, 2024 -->
<!-- Version 121.0.2277.83: January 25, 2024, 2023 to Version 121.0.2277.4: December 15, 2023 -->
<!-- Version 120.0.2210.61: December 7, 2023 to Version 120.0.2210.7: November 13, 2023 -->
<!-- Version 119.0.2151.44: November 2, 2023, 2023 to Version 119.0.2151.24: October 23, 2023 -->
<!-- Version 119.0.2151.12: October 17, 2023 to Version 118.0.2088.17: September 25, 2023 -->
<!-- Version 118.0.2088.11: September 20, 2023 to Version 117.0.2045.12: August 29, 2023 -->
<!-- Version 117.0.2045.9: August 25, 2023 to Version 116.0.1938.36: July 31, 2023 -->
<!-- Version 116.0.1938.29: July 24, 2023 to Version 115.0.1901.9: June 15, 2023 -->
<!-- from Version 115.0.1901.7: June 13, 2023 to Version 114.0.1823.18: May 15, 2023 -->
<!-- Version 114.0.1823.11: May 9, 2023 to Version 113.0.1774.15: April 18, 2023 -->
<!-- Version 113.0.1774.9: April 12, 2023 to Version 112.0.1722.15: March 21, 2023 -->
<!-- from Version 112.0.1722.11: March 17, 2023 to Version 111.0.1661.22: February 24, 2023 -->
<!-- from Version 111.0.1661.15: February 16, 2023 to Version 110.0.1587.22: January 24, 2023 -->
<!--- from Version 110.0.1587.17: January 20, 2023 to Version 109.0.1518.23: December 14, 2022 -->
<!--- from Version 109.0.1518.14: December 7, 2022 to Version 108.0.1462.20: November 14, 2022 -->
<!--- from Version 108.0.1462.15: November 10, 2022 to Version 107.0.1418.13: October 18, 2022 -->
<!--- from Version 107.0.1418.8: October 13, 2022 to Version 106.0.1370.17: September 16, 2022 -->
<!-- from Version 106.0.1370.15: September 15, 2022 to Version Version 105.0.1343.10: August 19, 2022 ---->
<!--- from Version 105.0.1343.7: August 16, 2022 to Version 104.0.1293.21: July 14 ---->
<!--- from Version 104.0.1293.14: July 7 to Version 103.0.1264.17: June 6 ---->
<!--- from Version 103.0.1264.13: June 2 to Version 102.0.1245.12: May 13 ---->
<!--- from Version 102.0.1245.7: May 10 to Version 101.0.1210.14: April 12 ---->
<!--- from Version 101.0.1210.10: April 8 to Version 100.0.1185.12: March 18 --->
<!--- from Version 100.0.1185.10: March 17 to Version 99.0.1150.16: February 14 --->
<!--- From Version 99.0.1150.11: February 9 to Version 98.0.1108.27: January 19 --->
<!-- archive from Version 98.0.1108.23: January 14 to Version 97.0.1072.28: December 8 -->
<!--- Version 97.0.1072.21: December 1 to Version 96.0.1054.13: November 5  --->
<!--- archive from Version 96.0.1054.8: November 1 to Version 95.0.1020.14: October 5  --->
<!-- archive from version 95.0.1020.9: September 28 to version 94.0.992.14: September 7 -->
<!-- archive from Version 94.0.992.9: September 2 to Version 92.0.902.40: July 6 -->
<!--Archive from Version 92.0.902.22: June 21 to Version 89.0.774.23: February 8  -->
<!-- Archive from Version 87.0.664.18: October 26 to to version 89.0.774.18: February 3 --->
<!-- Archive from Version 87.0.664.12: October 20 to version 86.0.622.15: September 14 -->
<!--- Archived to version 86.0.622.11: September 9 ---->
<!--- Archived to version 85.0.564.18: July 28 ---->

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
