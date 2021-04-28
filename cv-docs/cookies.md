---
title: "Cookies in Dynamics 365 Customer Voice | MicrosoftDocs"
description: "Know the cookies used by Dynamics 365 Customer Voice"
ms.date: 02/18/2021
ms.service: dynamics-365-customervoice
ms.topic: article
author: sbmjais
ms.author: shjais
manager: shujoshi
---

# Cookies in Dynamics 365 Customer Voice

A cookie is a small file sent from the web site to visitor's device by the browser. A single web session may use multiple cookies.

Dynamics 365 Customer Voice also use cookies to store information for various purposes. The following table describes the cookies that Dynamics 365 Customer Voice uses, and their lifetime.

| Cookie name | Description | Lifetime |
|-------------|-------------|----------|
| AADNonce.forms | Unique identifier of one authentication session to prevent replay. | Session |
| DcLcid  | Saves language preference. | 90 days |
| MS0 | Stores the session identification cookie. | 90 days |
| MSFPC  | Critical service cookie to analyze service usage anonymously and aggregated for statistical purpose.   | 1 year |
|  MUID  | Used to identify different anonymous users. Critical service cookie to analyze service usage anonymously and aggregated for statistical purpose. | 1 year |
| _RequestVerificationToken  | Used by the [antiforgery](/dotnet/api/system.web.helpers.antiforgeryconfig.cookiename) system.  | Session |
| AADAuth.forms | Azure Active Directory authentication token. | 90 days |
| AADAuthCode.forms | An authentication code used to redeem Azure Active Directory authentication token. | 90 days |
| AADSID.forms | Azure Active Directory authentication session ID.  | 90 days |
| AADState.forms | Authentication state to indicate whether user is authenticated. | 90 days |
||||


[!INCLUDE[footer-include](includes/footer-banner.md)]
