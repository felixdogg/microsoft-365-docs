---
title: Supported Microsoft Defender XDR APIs
description: Supported Microsoft Defender XDR APIs
ms.service: defender-xdr
f1.keywords: 
  - NOCSH
ms.author: macapara
author: mjcaparas
ms.localizationpriority: medium
manager: dansimp
audience: ITPro
ms.collection: 
 - m365-security
 - tier3
 - must-keep
ms.topic: reference
search.appverid: 
  - MOE150
  - MET150
ms.custom: api
ms.date: 02/08/2024
---

# Supported Microsoft Defender XDR APIs

[!INCLUDE [Microsoft Defender XDR rebranding](../includes/microsoft-defender.md)]

**Applies to:**
- Microsoft Defender XDR

> [!NOTE]
> **Try our new APIs using MS Graph security API**. Find out more at: [Use the Microsoft Graph security API - Microsoft Graph | Microsoft Learn](/graph/api/resources/security-api-overview).

> [!IMPORTANT]
> Some information relates to prereleased product which may be substantially modified before it's commercially released. Microsoft makes no warranties, express or implied, with respect to the information provided here.

## List of available APIs

Article | Description
-|-
[Advanced Hunting API](api-advanced-hunting.md) | Run Advanced Hunting queries.
[Incident APIs](api-incident.md) | List and update incidents, along with other practical tasks.
[Streaming API](streaming-api.md) | Ship real-time events and alerts as they occur in a single data stream.

### Endpoint URIs

The base URI for both of the main APIs is: https://api.security.microsoft.com. For better performance, use a server closer to your geolocation:

- The United States: api-us.security.microsoft.com
- Europe: api-eu.security.microsoft.com
- The United Kingdom: api-uk.security.microsoft.com

Tokens can be acquired by accessing https://api.security.microsoft.com.

All APIs along the `/api` path use the [OData](/odata/overview) Protocol; for example, https://api.security.microsoft.com/api/incidents.

## Related articles

- [Use the Microsoft Graph security API - Microsoft Graph | Microsoft Learn](/graph/api/resources/security-api-overview)

- [Microsoft Defender XDR APIs overview](api-overview.md)
- [Access the Microsoft Defender XDR APIs](api-access.md)
- [Streaming API](../defender-endpoint/raw-data-export.md)
- [Learn about API limits and licensing](api-terms.md)
- [Understand error codes](api-error-codes.md)
[!INCLUDE [Microsoft Defender XDR rebranding](../../includes/defender-m3d-techcommunity.md)]
