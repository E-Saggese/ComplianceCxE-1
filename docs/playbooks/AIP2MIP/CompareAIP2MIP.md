# Compare AIP Add-In with Built-In Labeling in M365 Apps
Many of the labeling features supported by the AIP add-in are now supported by built-in labeling. The table below is an adaptation of [Feature parity for built-in labeling and the AIP add-in for Office apps](https://learn.microsoft.com/en-us/microsoft-365/compliance/sensitivity-labels-aip#feature-parity-for-built-in-labeling-and-the-aip-add-in-for-office-apps) and offers additional information to help you prepare your transition from the AIP add-in. 

> 🗒️ Note: For a more detailed list of capabilities, minimum versions that might be needed, and configuration information, see [Manage sensitivity labels in Office apps](https://learn.microsoft.com/en-us/microsoft-365/compliance/sensitivity-labels-office-apps?view=o365-worldwide).

### Feature Roadmap
The following categories help you identify the support status for Add-in functionality available in built-in labeling.

- `✅ Supported`: General availability in [Current Channel](https://learn.microsoft.com/en-us/deployoffice/overview-update-channels#current-channel-overview)
- `⭐ In Preview`: Available in [Insider Beta Channel](https://learn.microsoft.com/en-us/DeployOffice/office-insider/compare-channels) to try now. Provides a `📅 M365 Roadmap` tracking item.
- `🔷 In Development`: Development is under way. Keep an eye out for product roadmap updates. General availability **3-6 months** time horizon. Provides a `📅 M365 Roadmap` tracking item.
- `🟨 In Planning`: In consideration for an upcoming development cycle, but not yet commited on product roadmap. General availability **6-12 months** time horizon.
- `⚫ Not Planned`: Items that are not in consideration for built-in labeling. Submit a Microsoft support ticket for a Design Change Request (DCR) if these are important for your organization.
- `🟢 Not Needed`: Items that are only needed to workaround limitations of an add-in; not needed for built-in labeling

### Change Management Insights
To help you plan your migration, the following "traffic light" ranks degrees of change that compliance IT admins and end-users/information workers can expect when transitioning from AIP Add-In (Current) to Built-In (Current), to Built-In (Coming Soon).

- `🟢⚪⚪`: Fully Supported. Minor differences may exist, but does not require configuration changes or proactive end-user education (aka "silent change").
- `⚪🟡⚪`: Supported with minor differences. No configuration changes required, but may need updates to training, support docs, or end-user comms. Targeted testing recommended.
- `⚪⚠️⚪`: Supported, but requires changes to policy configuration and/or broad testing.
- `⚪⚪⭕`: Supported with alternative solutions available from Microsoft (e.g. AIP Classify & Protect, SPO Auto Labeling)
- `⚪⚪🚫`: Not Supported.
- `⚪⚪⚪`: No change from prior state.

The migration guides available for most features provides additional details about the changes to expect and how to prepare.

-----

## Azure Information Protection Add-in Scenarios
Review the list of scenarios and their availability in built-in labeling below. Where available, references to additional resources are provided.

| Scenario Refernce | Roadmap | Change Management | 
|:-----|:-----|:-----|
| 🖥️ **Labeling Environment** | | |
| Choose a labeling client for Office<br>- Support: [👮 Admin](https://learn.microsoft.com/en-us/microsoft-365/compliance/sensitivity-labels-office-apps#if-you-need-to-turn-off-built-in-labeling-in-office-apps-on-windows) | `✅ Supported` | 📖[**Change Guide**](Features/Environment/ConfigureLabelingClient.md) *`(New)`*<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: ⚪⚠️⚪`<br>- `Built-In v2211: ⚪⚠️⚪` | 
| Labeling for modern Office files in Open XML format (e.g. docx) <br>- Support: [👮 Admin](https://learn.microsoft.com/en-us/microsoft-365/compliance/sensitivity-labels-office-apps?view=o365-worldwide#office-file-types-supported)| `✅ Supported` | 📖 [**Change Guide**](Features/Environment/FileTypeSupport.md) *`(New)`*<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: 🟢⚪⚪`<br>- `Built-In vSOON: 🟢⚪⚪` |  
| View and apply sensitivity labels in government cloud | `✅ Supported` | - `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: 🟢⚪⚪` |
| Admin can scope labels independently for files and emails | `🔷 In Development`<br>[📅 M365 Roadmap 99939](https://www.microsoft.com/en-us/microsoft-365/roadmap?filters=&searchterms=99939) <br>| 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: ⚪⚪🚫`<br>- `Built-In v1910: ⚪⚪🚫`<br>- `Built-In vSOON: ⚪⚠️⚪` |  
| Labeling for legacy Office files in Microsoft Office 97-2003 format (e.g. doc) <br>- Support: [➡️ AIP Reference](https://learn.microsoft.com/en-us/microsoft-365/compliance/sensitivity-labels-office-apps?view=o365-worldwide#office-file-types-supported)| `⚫ Not Planned` | 📖 [**Change Guide**](Features/Environment/FileTypeSupport.md) *`(New)`*<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: ⚪⚪⭕`| 
| Support for labeling using Office perpetual <br>- Support: [👮 Admin](https://learn.microsoft.com/en-us/microsoft-365/compliance/sensitivity-labels-office-apps#labeling-client-for-desktop-apps)| `⚫ Not Planned`| 📖 [**Change Guide**](Features/Environment/OfficeEditions.md) *`(New)`*<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: ⚪⚪🚫` | 
| | |
| 🧑‍💻 **Labeling User Experience**  | | | 
| Sensitivity Status <br> - Support: [🧑‍💻 User](https://support.microsoft.com/en-us/office/apply-sensitivity-labels-to-your-files-and-email-in-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9) | `✅ Supported` | 📖 [**Change Guide**](Features/UX/SensitivityStatus.md) *`(New)`*<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: 🟢⚪⚪`<br>- `Built-In v2211: 🟢⚪⚪` | 
| Sensitivity menu (ribbon) <br>- Support: [🧑‍💻 User](https://support.microsoft.com/en-us/office/apply-sensitivity-labels-to-your-files-and-email-in-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9)| `✅ Supported` | 📖 [**Change Guide**](Features/UX/SensitivityMenu.md) *`(New)`*<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: 🟢⚪⚪`<br>- `Built-In v2211: 🟢⚪⚪` | 
| Multilanguage label names and descriptions <br>- Support: [👮 Admin](https://learn.microsoft.com/en-us/microsoft-365/compliance/create-sensitivity-labels) | `✅ Supported` | - `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: 🟢⚪⚪` | 
| Sensitivity bar <br>- Support: [👮 Admin](https://learn.microsoft.com/en-us/microsoft-365/compliance/sensitivity-labels-office-apps?view=o365-worldwide#sensitivity-bar), [🧑‍💻 User](https://support.microsoft.com/en-us/office/apply-sensitivity-labels-to-your-files-and-email-in-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9)| `⭐ In Preview`<br>[📅 M365 Roadmap 88517](https://www.microsoft.com/en-us/microsoft-365/roadmap?filters=&searchterms=88517)<br>[📣 Office Insiders Blog](https://insider.office.com/en-us/blog/sensitivity-bar-in-office-for-windows) | 📖 [**Change Guide**](Features/UX/SensitivityBar.md) *`(New)`*<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: ⚪⚪🚫`<br>- `Built-In vSOON: ⚪🟡⚪` | 
| Label Colors | `⭐ In Preview`<br>[📅 M365 Roadmap 93217](https://www.microsoft.com/en-us/microsoft-365/roadmap?filters=&searchterms=93217) | 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: ⚪⚪🚫`<br>- `Built-In vSOON: 🟢⚪⚪` | 
| | | |
| ⚠️ **Labeling Enforcement** | | | | 
| Manual labeling <br>- Support: [🧑‍💻 User](https://support.microsoft.com/en-us/office/apply-sensitivity-labels-to-your-files-and-email-in-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9) | `✅ Supported` | 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: ⚪🟡⚪`<br>- `Built-In vSOON: 🟢⚪⚪` | 
| Mandatory labeling: Enforce at file-save<br>- Support: [👮 Admin](https://learn.microsoft.com/en-us/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide#what-label-policies-can-do) |  `✅ Supported`| 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v2101: 🟢⚪⚪` | 
| Mandatory labeling: Files vs. Emails <br>- Support: [👮 Admin](https://learn.microsoft.com/en-us/microsoft-365/compliance/sensitivity-labels-office-apps?view=o365-worldwide#outlook-specific-options-for-default-label-and-mandatory-labeling) | `✅ Supported` | 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v2101: 🟢⚪⚪` | 
| Downgrade Justification <br>- Support: [👮 Admin](https://learn.microsoft.com/en-us/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide#what-label-policies-can-do), [🧑‍💻 User](https://support.microsoft.com/en-us/office/apply-sensitivity-labels-to-your-files-and-email-in-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9) | `✅ Supported` | 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: ⚪🟡⚪`<br>- `Built-In v2206: 🟢⚪⚪` | 
| Manual Labeling: Preselect default sublabel<br>- Support: [➡️ AIP Reference](https://learn.microsoft.com/en-us/azure/information-protection/rms-client/clientv2-admin-guide-customizations#specify-a-default-sublabel-for-a-parent-label) | `🟨 In Planning` <br>📅  Roadmap `Coming soon`| 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: ⚪⚪🚫`<br>- `Built-In vSOON: 🟢⚪⚪` | 
| Mandatory labeling: Enforcement at app close [➡️ Reference](https://learn.microsoft.com/en-us/azure/information-protection/rms-client/clientv2-admin-guide-customizations#remove-not-now-for-documents-when-you-use-mandatory-labeling) | `🟨 In Planning` <br>📅  Roadmap `Coming soon`| 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v2101: ⚪⚪🚫`<br>- `Built-In vSOON: 🟢⚪⚪` | 
| | |
| ⚡ **Labeling Automation** | | | 
| Default Labeling: Files<br>- Support: [👮 Admin](https://learn.microsoft.com/en-us/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide#what-label-policies-can-do)| `✅ Supported` | 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: ⚪🟡⚪`<br>- `Built-In v2208: 🟢⚪⚪` | 
| Default Labeling: Emails <br>- Support: [👮 Admin](https://learn.microsoft.com/en-us/microsoft-365/compliance/sensitivity-labels-office-apps?view=o365-worldwide#outlook-specific-options-for-default-label-and-mandatory-labeling)| `✅ Supported` | 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: 🟢⚪⚪` | 
| Automatic or recommended labeling of files and emails with sensitive information types <br>- Support:[👮 Admin](https://learn.microsoft.com/en-us/microsoft-365/compliance/apply-sensitivity-label-automatically?view=o365-worldwide) | `✅ Supported` | 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In 2009: 🟢⚪⚪` | 
| Automatic or recommended labeling of emails based on attachment labels <br>- Support: [➡️ AIP Reference](https://learn.microsoft.com/en-us/azure/information-protection/rms-client/clientv2-admin-guide-customizations#for-email-messages-with-attachments-apply-a-label-that-matches-the-highest-classification-of-those-attachments) | `🔷 In Development`<br> [📅 M365 Roadmap 100490](https://www.microsoft.com/en-us/microsoft-365/roadmap?filters=&searchterms=100490) | 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: ⚪⚪🚫`<br>- `Built-In vSOON: ⚪🟡⚪` | 
| | |
| 🔒 **Encryption as an outcome for labeling** | | | 
| Admin-defined permissions <br>- Support: [👮 Admin](https://learn.microsoft.com/en-us/microsoft-365/compliance/encryption-sensitivity-labels?view=o365-worldwide#assign-permissions-now) | `✅ Supported` | 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: 🟢⚪⚪` | 
| User-defined permissions: Files restricted to users and groups <br>- Support: [👮 Admin](https://learn.microsoft.com/en-us/microsoft-365/compliance/encryption-sensitivity-labels?view=o365-worldwide#let-users-assign-permissions) | `✅ Supported` | 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v2004: ⚪🟡⚪` | 
| User-defined permissions: Do Not Forward for emails <br>- Support: [👮 Admin](https://learn.microsoft.com/en-us/azure/information-protection/configure-usage-rights#do-not-forward-option-for-emails) | `✅ Supported` | 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: 🟢⚪⚪` | 
| User-defined permissions: Files restricted to domain names <br>- Support: [👮 Admin](https://learn.microsoft.com/en-us/microsoft-365/compliance/encryption-sensitivity-labels?view=o365-worldwide#support-for-organization-wide-custom-permissions) | `⭐ In Preview`<br>[📅 M365 Roadmap 98131](https://www.microsoft.com/en-us/microsoft-365/roadmap?filters=&searchterms=98131) | 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: ⚪⚪🚫`<br>- `Built-In vSOON: 🟢⚪⚪` | 
| S/MIME for emails <br>- Support: [👮 Admin](https://learn.microsoft.com/en-us/microsoft-365/compliance/sensitivity-labels-office-apps?view=o365-worldwide#configure-a-label-to-apply-smime-protection-in-outlook)| `⭐ In Preview`<br>[📅 M365 Roadmap 100062](https://www.microsoft.com/en-us/microsoft-365/roadmap?filters=&searchterms=100062) | 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: ⚪⚪🚫`<br>- `Built-In vSOON: ⚪🟡⚪` | 
| Double Key Encryption <br>- Support: [➡️ AIP Reference](https://learn.microsoft.com/en-us/microsoft-365/compliance/double-key-encryption-overview?view=o365-worldwide#can-i-use-double-key-encryption-with-microsoft-office-built-in-sensitivity-labeling)| `🟨 In Planning` <br>📅  Roadmap `Coming soon`| 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: ⚪⚪🚫`<br>- `Built-In vSOON: ⚪⚠️⚪` | 
| Document Tracking & Revocation for Compliance Admins <br>- Support: [➡️ AIP Reference](https://learn.microsoft.com/en-us/azure/information-protection/rms-client/track-and-revoke-admin)| `🟨 In Planning` <br>📅  Roadmap `Coming soon`| 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: ⚪⚪🚫`<br>- `Built-In vSOON: ⚪⚠️⚪` | 
| Document Revocation for End-Users <br>- Support: [➡️ AIP Reference](https://learn.microsoft.com/en-us/azure/information-protection/rms-client/revoke-access-user#revoke-access-from-microsoft-office-apps)| `🟨 In Planning` <br>📅  Roadmap `Coming soon`| 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: ⚪⚪🚫`<br>- `Built-In vSOON: ⚪⚠️⚪` | 
| | |
| 📨 **Collaboration with labeled content** | | | 
| Multi-user editing of encrypted files<br>- Support: [👮 Admin](https://learn.microsoft.com/en-us/microsoft-365/compliance/sensitivity-labels-coauthoring) | `✅ Supported` | 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: ⚪⚪🚫`<br>- `Built-In v2107: 🟢⚪⚪` | 
| Block/warn/justify before sending emails<br>- Support: [➡️ AIP Reference](https://learn.microsoft.com/en-us/azure/information-protection/rms-client/clientv2-admin-guide-customizations#implement-pop-up-messages-in-outlook-that-warn-justify-or-block-emails-being-sent) | `🔷 In Development`<br>[📅 M365 Roadmap 100255](https://www.microsoft.com/en-us/microsoft-365/roadmap?filters=&searchterms=100255) | 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: ⚪⚪🚫`<br>- `Built-In vSOON: ⚪⚠️⚪` | 
| | |
| 🏷️ **Content Marking** | | | 
| Headers, footers, watermark<br>- Support: [👮 Admin](https://learn.microsoft.com/en-us/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide#what-sensitivity-labels-can-do) | `✅ Supported` | 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: ⚪🟡⚪`<br>- `Built-In vSOON: 🟢⚪⚪` | 
| Dynamic markings<br>- Support: [👮 Admin](https://learn.microsoft.com/en-us/microsoft-365/compliance/sensitivity-labels-office-apps?view=o365-worldwide#dynamic-markings-with-variables) | `✅ Supported` | 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: ⚪⚪🚫`<br>- `Built-In v2010: 🟢⚪⚪` | 
| Per app visual marking<br>- Support: [👮 Admin](https://learn.microsoft.com/en-us/microsoft-365/compliance/sensitivity-labels-office-apps?view=o365-worldwide#setting-different-visual-markings-for-word-excel-powerpoint-and-outlook) | `✅ Supported` | 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: ⚪⚪🚫`<br>- `Built-In v2010: 🟢⚪⚪` | 
| | |
| 📊 **Reporting and Analytics** | | | 
| Disable Auditing<br>- Support: [👮 Admin](https://review.learn.microsoft.com/en-us/powershell/module/exchange/set-labelpolicy?view=exchange-ps#-advancedsettings) | `✅ Supported` | 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: ⚪⚪🚫`<br>- `Built-In v2011: 🟢⚪⚪` | 
| Auditing labeling activities <br>- Support: [👮 Admin](https://learn.microsoft.com/en-us/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance?view=o365-worldwide#sensitivity-label-activities) | `✅ Supported` | 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: ⚪🟡⚪`<br>- `Built-In vSOON: 🟢⚪⚪` | 
| | |
| 🔀 **Migrate from alternative labeling clients** | | | 
| Label by custom properties<br>- Support: [➡️ AIP Reference](https://learn.microsoft.com/en-us/azure/information-protection/rms-client/clientv2-admin-guide-customizations#migrate-labels-from-secure-islands-and-other-labeling-solutions) | `⚫ Not Planned` | 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: ⚪⚪⭕` |
| Remove external markings<br>- Support: [➡️ AIP Reference](https://learn.microsoft.com/en-us/azure/information-protection/rms-client/clientv2-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions) | `⚫ Not Planned` | 📖 Change Guide `[Coming Soon]`<br>- `Add-In vLATEST: 🟢⚪⚪`<br>- `Built-In v1910: ⚪⚪⭕` | 
|  | ~~~~~~~~~~~~~~~~~~~ | ~~~~~~~~~~~~~~~~~~~~~~~~ | 

