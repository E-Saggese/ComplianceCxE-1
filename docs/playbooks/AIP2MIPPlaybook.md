![image](https://user-images.githubusercontent.com/43501191/195164735-920ec45a-cd2c-41a1-9d22-6a557ca9ddc3.png)


# From bolt-on to built-in – Migrate from Azure Information Protection Add-in 

## Overview

Office apps have supported sensitivity labels [since September 2018](https://techcommunity.microsoft.com/t5/security-compliance-and-identity/azure-information-protection-is-now-generally-available/ba-p/249974), starting in Office for PC, using [Azure Information Protection (AIP) Add-in](https://learn.microsoft.com/en-us/azure/information-protection/rms-client/aip-clientv2). In October 2019, Office apps started providing the [same functionality built into Word, Excel, PowerPoint, and Outlook](https://learn.microsoft.com/en-us/microsoft-365/compliance/sensitivity-labels-office-apps#support-for-sensitivity-label-capabilities-in-apps) and expanded sensitivity labels across Mac, Web, and Mobile for comprehensive, consistent, and seamless experience for end-users and admins.

## Built-In Instead of Bolt-On

Built-in labeling forms the cornerstone of a [Microsoft Purview information protection deployment](https://learn.microsoft.com/en-us/microsoft-365/compliance/information-protection-solution?view=o365-worldwide) it extends across platforms (Windows, macOS, iOS, Android, and web), as well as across Microsoft apps and services, and beyond. Built-in labeling is also designed to work with other Microsoft Purview capabilities, such as data classification and Microsoft Purview data loss prevention (DLP).

Customers benefited from the choice between the AIP add-in or the built-in native labeling [depending on the features they needed](https://learn.microsoft.com/en-us/microsoft-365/compliance/sensitivity-labels-aip?view=o365-worldwide#feature-parity-for-built-in-labeling-and-the-aip-add-in-for-office-apps), but this also created challenges and tradeoffs for organizations:

| Add-In Limitations | Degrades end-user productivity and satisfaction |  Higher cost for IT
|:---|:---|:---|
| 🔓 Add-in can be disabled by end-users, leaving your data potentially vulnerable.<br>🛑 Add-in features are “frozen in time” since December 2021 at the start of its maintenance period. | 🐢 Like most add-ins, AIP regularly impacts end-user productivity because of performance implications with the add-in. <br>📱 Users of Office on other platforms face inconsistencies with sensitivity labeling since the Add-in only supports Office for PC. | ⚙️ AIP Add-in requires separate configuration, deployment, and management from the rest of the admin experience.|

Read the blog “[From bolt-on to built-in information protection in Microsoft 365 Apps](https://aka.ms/AIP2MIP/Newsletter)” for an overview about this change.

> ⚠️ Warning: Up until recently, built-in labeling was turned off by default in Office for Windows apps when the AIP client was installed. This default will no longer be the case for newer versions of Office. Soon, the built-in labeling will become the default. Learn more about the [change of default labeling client and how to configure your preferred labeling client](https://learn.microsoft.com/en-us/microsoft-365/compliance/sensitivity-labels-aip).


> 💡 Tip: You can continue using all other tools in the AIP client, such as the Scanner, PowerShell extensions, or Windows right-click extension Classify & Protect. These tools are not affected by disabling the add-in inside Office and continue to be the recommended tools for all your sensitivity labeling scenarios that aren’t available within the Office apps.

## Get Started

For customers currently using the AIP Add-in for Office, use the playbooks below to help you plan and execute the transition to built-in labeling in Office apps. It provides a centralized resource to guide you through the prerequisites, configuration, and deployment of the built-in sensitivity labels in Office. 

| Self-Evaluation | Migration Playbook | Comparison Guide |
| :----- | :----- | :----- | 
| Try an interactive questionnaire that tailors the migration guide to your organization's needs.<br><br><p align="center"><a href="https://aka.ms/AIP2MIP/Guide/Evaluate" target="_blank"><img src="https://user-images.githubusercontent.com/43501191/195224353-b8263be1-7a68-40fe-ab2c-aa524da8bd84.png" alt="Self-Evaluation Guide"/></a></p> | Review a simple 5-step guide to help you learn, evaluate, and execute replacement of the AIP Add-in.<br><br><p align="center"><a href="../AIP2MIP/GetStarted" ><img src="https://user-images.githubusercontent.com/43501191/195224310-e7cc634b-01f8-4f28-b13f-45d1dc582d7b.png" alt="Migration Playbook"/></a></p> | Comprehensive roadmap and change-management guidelines each capability in the AIP add-in relative to its replacement in built-in labeling.<br><br><p align="center"><a href="../AIP2MIP/CompareAIP2MIP" ><img src="https://user-images.githubusercontent.com/43501191/195224282-2717594a-1d79-4cd7-a30a-4d6a22d1da6a.png" alt="Comparison Guide"/></a></p>|

-------------

## Get Help

We recommend you join the Microsoft Purview [Customer Community Program (CCP)](https://aka.ms/JoinCompliancePrivacyCCP) for access to demos from the product teams, webinars from experts, and private previews that give you early access to all sensitivity labeling features that are coming soon to built-in labeling in Office.

If you need additional assistance to evaluate how to migrate users using the AIP Add-in after reviewing the migration guide, reach out to [AIP2MIPGetHelp](mailto:AIP2MIPGetHelp@microsoft.com). We will do our best to respond to inquiries and direct you to the appropriate support resources for your organization.
