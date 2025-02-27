---
title: How to subscribe to Microsoft Defender Experts for Hunting
ms.reviewer:
description: If you're new to Microsoft Defender XDR and Defender Experts for Hunting, this is how you onboard, receive, and set up Defender experts notifications.
keywords: managed threat hunting service,onboarding to Defender Experts, sample DEN, defender experts notifications, Ask Defender Experts, MTE, Microsoft Threat Experts, EOD, endpoint attack notifications, Microsoft Defender Experts for hunting, managed response.
search.product: Windows 10
ms.service: defender-experts
ms.mktglfcycl: deploy
ms.sitesec: library
ms.pagetype: security
ms.author: vpattnaik
author: vpattnai
ms.localizationpriority: medium
manager: dansimp
audience: ITPro
ms.collection:
  - m365-security
  - tier1
  - essentials-get-started
ms.topic: conceptual
search.appverid: met150
ms.date: 04/08/2024
---

# Start using Microsoft Defender Experts for Hunting

[!INCLUDE [Microsoft Defender XDR rebranding](../../includes/microsoft-defender.md)]

**Applies to:**

- [Microsoft Defender XDR](https://go.microsoft.com/fwlink/?linkid=2118804)

## Onboarding

If you're new to Microsoft Defender XDR and Defender Experts for Hunting:

1. Upon getting your welcome email, select **Log into Microsoft Defender XDR**.
2. Sign in if you already have a Microsoft account. If none, create one.
3. The Microsoft Defender XDR quick tour gets you familiar with the security suite, where the capabilities are and how important they are. Select **Take a quick tour**.
4. Read the short descriptions about what the Microsoft Defender Experts service is and the capabilities it provides. Select **Next**. You see the welcome page:

![Screenshot of the Microsoft Defender XDR welcome page with a card for the Defender Experts for Hunting service.](../../media/mte/defenderexperts/start-using-defender-experts-for-hunting.png)

## Receive Defender Experts Notifications

The Defender Experts Notifications service includes:

- Threat monitoring and analysis, reducing dwell time and the risk to your business
- Hunter-trained artificial intelligence to discover and target both known attacks and emerging threats
- Identification of the most pertinent risks, helping SOCs maximize their effectiveness
- Help in scoping compromises and as much context as can be quickly delivered to enable a swift SOC response

Refer to the following screenshot to see a sample Defender Experts Notification:

![Screenshot of a Defender Experts Notification in Microsoft Defender XDR. A Defender Expert Notification includes a title that describes the threat or activity observed, an executive summary, and list of recommendations.](../../media/mte/defenderexperts/receive-defender-experts-notification.png)

### Where to find Defender Experts Notifications

You can receive Defender Experts Notifications from Defender Experts through the following mediums:

- The Microsoft Defender portal's [Incidents](https://security.microsoft.com/incidents) page
- The Microsoft Defender portal's [Alerts](https://security.microsoft.com/alerts) page
- OData alerting [API](../../security/defender-endpoint/get-alerts.md) and [REST API](../defender-endpoint/configure-siem.md)
- [DeviceAlertEvents](../../security/defender-endpoint/advanced-hunting-devicealertevents-table.md) table in Advanced hunting
- Your email if you [configure an email notifications rule](/microsoft-365/security/defender/onboarding-defender-experts-for-hunting#set-up-defender-experts-email-notifications)

### Filter to view just the Defender Experts Notifications

You can filter your incidents and alerts if you want to only see the Defender Experts Notifications among the many alerts. To do so:

1. On the navigation menu, go to **Incidents & alerts** > **Incidents** > select the ![Filter icon](../../media/mte/defenderexperts/filter.png) icon.
2. Scroll down to **Service/detection sources** then select the **Microsoft Defender Experts** checkboxes under *Microsoft Defender for Endpoint* and *Microsoft Defender XDR*.
3. Select **Apply**.

### Set up Defender Experts email notifications

You can set up Microsoft Defender XDR to notify you or your staff with an email about new incidents or updates to existing incidents, including those observed by Microsoft Defender Experts. [Learn more about getting incident notifications by email](/microsoft-365/security/defender/incidents-overview#get-incident-notifications-by-email)

1. In the Microsoft Defender XDR navigation pane, select **Settings** > **Microsoft Defender XDR** > **Email notifications** > **Incidents**.
2. Update your existing email notification rules or create a new one. [Learn more about creating a rule for email notifications](/microsoft-365/security/defender/incidents-overview#create-a-rule-for-email-notifications)
3. On the rule's **Notification settings** page, make sure to configure the following:
    - **Source** – Choose **Microsoft Defender Experts** under **Microsoft Defender XDR** and **Microsoft Defender for Endpoint**
    - **Alert severity** – Choose the alert severities that will trigger an incident notification. For example, if you only want to be informed about high-severity incidents, select High.

### Generate sample Defender Experts Notifications

You can generate a sample Defender Experts Notification to start experiencing the Defender Experts for Hunting service without having to wait for an actual critical activity to happen in your environment. Generating a sample notification also lets you test the [email notifications](#set-up-defender-experts-email-notifications) you might have previously configured in the Microsoft Defender portal for this service, as well as test the configuration of playbooks (if configured for such notifications) and rules in your Security Information and Event Management (SIEM) environment.

A sample Defender Experts Notification shows up in your **Incidents** page with the title _Defender Experts: Test Notification from Microsoft Defender Experts_. The [contents](#receive-defender-experts-notifications) of the notification are placeholder texts, while the other elements such as alerts are randomly generated from events present in your tenant and aren't actually impacted.

:::image type="content" source="../../media/mte/defenderexperts/sample-den-dexh.png" alt-text="Screenshot of Sample DEN in Defender Experts for Hunting." lightbox="../../media/mte/defenderexperts/sample-den-dexh.png":::

**To generate a sample notification:**

1. In your Microsoft Defender XDR navigation pane, go to **Settings** > **Defender Experts** and then select **Sample notifications**.
2. Select **Generate a sample notification**. A green status message appears, confirming that your sample notification is ready for review.
3. Under **Recently generated Defender Experts Notification**, select a link from the list to view its corresponding generated sample notification. The most recent sample appears on the top of the list. Selecting a link redirects you to the **Incidents** page.

:::image type="content" source="../../media/mte/defenderexperts/sample-den-links-dexh.png" alt-text="Screenshot of Sample DEN links." lightbox="../../media/mte/defenderexperts/sample-den-links-dexh.png":::

## Collaborate with experts on demand

> [!NOTE]
> Ask Defender Experts is included in your Defender Experts for Hunting subscription with [monthly allocations](/microsoft-365/security/defender/before-you-begin-defender-experts#eligibility-and-licensing). However, it's not a security incident response service. It's intended to provide a better understanding of complex threats affecting your organization. Engage with your own security incident response team to address urgent security incident response issues. If you don't have your own security incident response team and would like Microsoft's help, create a support request in the [Premier Services Hub](/services-hub/).

Select **Ask Defender Experts** directly inside the Microsoft 365 security portal to get swift and accurate responses to all your threat hunting questions. Experts can provide insight to better understand the complex threats your organization might face. Ask Defender Experts can help:

- Gather additional information on alerts and incidents, including root causes and scope
- Gain clarity into suspicious devices, alerts, or incidents and take next steps if faced with an advanced attacker
- Determine risks and available protections related to threat actors, campaigns, or emerging attacker techniques

### Required permissions for submitting inquiries in the Ask Defender Experts panel

You need to select the following permissions before submitting inquires to our Defender experts. For more details about role-based access control (RBAC) permissions, see: [Microsoft Defender for Endpoint and Microsoft Defender XDR RBAC permissions](/microsoft-365/security/defender/compare-rbac-roles#map-defender-for-endpoint-and-defender-vulnerability-management-permissions-to-the-microsoft-defender-xdr-rbac-permissions).

|**Product name**|**Product RBAC permission**|
|---|---|---|
| Microsoft Defender for Endpoint RBAC | Manage security settings in the Security Center|
| Microsoft Defender XDR Unified RBAC | Authorization and settings \ Security settings \ Core security settings (manage)</br>Authorization and settings \ Security settings \ Detection tuning (manage) |

### Where to find Ask Defender Experts

The option to **Ask Defender Experts** is available in several places throughout the portal:

- **Device page actions menu**

   ![Screenshot of the Ask Defender Experts menu option in the Device page action menu in the Microsoft Defender portal.](../../media/mte/defenderexperts/device-page-actions-menu.png)

- **Device inventory page flyout menu**

   ![Screenshot of the Ask Defender Experts menu option in the Device inventory page flyout menu in the Microsoft Defender portal.](../../media/mte/defenderexperts/device-inventory-flyout-menu.png)

- **Alerts page flyout menu**

   ![Screenshot of the Ask Defender Experts menu option in the Alerts page flyout menu in the Microsoft Defender portal.](../../media/mte/defenderexperts/alerts-flyout-menu.png)

- **Incidents page actions menu**

   ![Screenshot of the Ask Defender Experts menu option in the Incidents page actions menu in the Microsoft Defender portal.](../../media/mte/defenderexperts/incidents-page-actions-menu.png)

### Sample questions you can ask from Defender Experts

**Alert information**

- We saw a new type of alert for a living-off-the-land binary. We can provide the alert ID. Can you tell us more about this alert and if it's related to any incident and how we can investigate it further?
- We've observed two similar attacks, which both try to execute malicious PowerShell scripts but generate different alerts. One is "Suspicious PowerShell command line" and the other is "A malicious file was detected based on indication provided by Office 365." What is the difference?
- We received an odd alert today about an abnormal number of failed logins from a high profile user's device. We can't find any further evidence for these attempts. How can Microsoft Defender XDR see these attempts? What type of logins are being monitored?
- Can you give more context or insight about the alert and any related incidents, "Suspicious behavior by a system utility was observed"?
- I observed an alert titled "Creation of forwarding/redirect rule". I believe the activity is benign. Can you tell me why I received an alert?

**Possible device compromise**

- Can you help explain why we see a message or alert for "Unknown process observed" on many devices in our organization? We appreciate any input to clarify whether this message or alert is related to malicious activity or incidents.
- Can you help validate a possible compromise on the following system, dating from last week? It's behaving similarly as a previous malware detection on the same system six months ago.

**Threat intelligence details**

- We detected a phishing email that delivered a malicious Word document to a user. The document caused a series of suspicious events, which triggered multiple alerts for a particular malware family. Do you have any information on this malware? If yes, can you send us a link?
- We recently saw a blog post about a threat that is targeting our industry. Can you help us understand what protection Microsoft Defender XDR provides against this threat actor?
- We recently observed a phishing campaign conducted against our organization. Can you tell us if this was targeted specifically to our company or vertical?

**Microsoft Defender Experts for Hunting alert communications**

- Can your incident response team help us address the Defender Experts Notification that we got?
- We received this Defender Experts Notification from Microsoft Defender Experts for Hunting. We don't have our own incident response team. What can we do now, and how can we contain the incident?
- We received a Defender Experts Notification from Microsoft Defender Experts for Hunting. What data can you provide to us that we can pass on to our incident response team?

### Next step

- [Understand the Defender Experts for Hunting report in Microsoft Defender XDR](defender-experts-report.md)
[!INCLUDE [Microsoft Defender XDR rebranding](../../includes/defender-m3d-techcommunity.md)]
