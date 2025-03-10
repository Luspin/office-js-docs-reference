---
title: Office.context.mailbox - requirement set 1.7
description: Outlook Mailbox API requirement set 1.7 version of the Mailbox object model.
ms.date: 04/01/2022
ms.localizationpriority: medium
---

# mailbox (requirement set 1.7)

### [Office](office.md)[.context](office.context.md).mailbox

Provides access to the Outlook add-in object model for Microsoft Outlook.

##### Requirements

|Requirement| Value|
|---|---|
|[Minimum mailbox requirement set version](../outlook-api-requirement-sets.md)| 1.1|
|[Minimum permission level](/office/dev/add-ins/outlook/understanding-outlook-add-in-permissions)| **restricted**|
|[Applicable Outlook mode](/office/dev/add-ins/outlook/outlook-add-ins-overview#extension-points)| Compose or Read|

## Properties

| Property | Minimum<br>permission level | Modes | Return type | Minimum<br>requirement set |
|---|---|---|---|:---:|
| [diagnostics](/javascript/api/outlook/office.mailbox?view=outlook-js-1.7&preserve-view=true#outlook-office-mailbox-diagnostics-member) | **read item** | Compose<br>Read | [Diagnostics](/javascript/api/outlook/office.diagnostics?view=outlook-js-1.7&preserve-view=true) | [1.1](../requirement-set-1.1/outlook-requirement-set-1.1.md) |
| [ewsUrl](/javascript/api/outlook/office.mailbox?view=outlook-js-1.7&preserve-view=true#outlook-office-mailbox-ewsurl-member) | **read item** | Compose<br>Read | String | [1.1](../requirement-set-1.1/outlook-requirement-set-1.1.md) |
| [item](office.context.mailbox.item.md) | **restricted** | Compose<br>Read | [Item](/javascript/api/outlook/office.item?view=outlook-js-1.7&preserve-view=true) | [1.1](../requirement-set-1.1/outlook-requirement-set-1.1.md) |
| [restUrl](/javascript/api/outlook/office.mailbox?view=outlook-js-1.7&preserve-view=true#outlook-office-mailbox-resturl-member) | **read item** | Compose<br>Read | String | [1.5](../requirement-set-1.5/outlook-requirement-set-1.5.md) |
| [userProfile](/javascript/api/outlook/office.mailbox?view=outlook-js-1.7&preserve-view=true#outlook-office-mailbox-userprofile-member) | **read item** | Compose<br>Read | [UserProfile](/javascript/api/outlook/office.userprofile?view=outlook-js-1.7&preserve-view=true) | [1.1](../requirement-set-1.1/outlook-requirement-set-1.1.md) |

## Methods

| Method | Minimum<br>permission level | Modes | Minimum<br>requirement set |
|---|---|---|:---:|
| [addHandlerAsync(eventType, handler, [options], [callback])](/javascript/api/outlook/office.mailbox?view=outlook-js-1.7&preserve-view=true#outlook-office-mailbox-addhandlerasync-member(1)) | **read item** | Compose<br>Read | [1.5](../requirement-set-1.5/outlook-requirement-set-1.5.md) |
| [convertToEwsId(itemId, restVersion)](/javascript/api/outlook/office.mailbox?view=outlook-js-1.7&preserve-view=true#outlook-office-mailbox-converttoewsid-member(1)) | **restricted** | Compose<br>Read | [1.3](../requirement-set-1.3/outlook-requirement-set-1.3.md) |
| [convertToLocalClientTime(timeValue)](/javascript/api/outlook/office.mailbox?view=outlook-js-1.7&preserve-view=true#outlook-office-mailbox-converttolocalclienttime-member(1)) | **read item** | Compose<br>Read | [1.1](../requirement-set-1.1/outlook-requirement-set-1.1.md) |
| [convertToRestId(itemId, restVersion)](/javascript/api/outlook/office.mailbox?view=outlook-js-1.7&preserve-view=true#outlook-office-mailbox-converttorestid-member(1)) | **restricted** | Compose<br>Read | [1.3](../requirement-set-1.3/outlook-requirement-set-1.3.md) |
| [convertToUtcClientTime(input)](/javascript/api/outlook/office.mailbox?view=outlook-js-1.7&preserve-view=true#outlook-office-mailbox-converttoutcclienttime-member(1)) | **read item** | Compose<br>Read | [1.1](../requirement-set-1.1/outlook-requirement-set-1.1.md) |
| [displayAppointmentForm(itemId)](/javascript/api/outlook/office.mailbox?view=outlook-js-1.7&preserve-view=true#outlook-office-mailbox-displayappointmentform-member(1)) | **read item** | Compose<br>Read | [1.1](../requirement-set-1.1/outlook-requirement-set-1.1.md) |
| [displayMessageForm(itemId)](/javascript/api/outlook/office.mailbox?view=outlook-js-1.7&preserve-view=true#outlook-office-mailbox-displaymessageform-member(1)) | **read item** | Compose<br>Read | [1.1](../requirement-set-1.1/outlook-requirement-set-1.1.md) |
| [displayNewAppointmentForm(parameters)](/javascript/api/outlook/office.mailbox?view=outlook-js-1.7&preserve-view=true#outlook-office-mailbox-displaynewappointmentform-member(1)) | **read item** | Read | [1.1](../requirement-set-1.1/outlook-requirement-set-1.1.md) |
| [displayNewMessageForm(parameters)](/javascript/api/outlook/office.mailbox?view=outlook-js-1.7&preserve-view=true#outlook-office-mailbox-displaynewmessageform-member(1)) | **read item** | Read | [1.6](../requirement-set-1.6/outlook-requirement-set-1.6.md) |
| [getCallbackTokenAsync([options], callback)](/javascript/api/outlook/office.mailbox?view=outlook-js-1.7&preserve-view=true#outlook-office-mailbox-getcallbacktokenasync-member(1)) | **read item** | Compose<br>Read | [1.5](../requirement-set-1.5/outlook-requirement-set-1.5.md) |
| [getCallbackTokenAsync(callback, [userContext])](/javascript/api/outlook/office.mailbox?view=outlook-js-1.7&preserve-view=true#outlook-office-mailbox-getcallbacktokenasync-member(2)) | **read item** | Compose<br>Read | [1.3](../requirement-set-1.3/outlook-requirement-set-1.3.md)<br>[1.1](../requirement-set-1.1/outlook-requirement-set-1.1.md) |
| [getUserIdentityTokenAsync(callback, [userContext])](/javascript/api/outlook/office.mailbox?view=outlook-js-1.7&preserve-view=true#outlook-office-mailbox-getuseridentitytokenasync-member(1)) | **read item** | Compose<br>Read | [1.1](../requirement-set-1.1/outlook-requirement-set-1.1.md) |
| [makeEwsRequestAsync(data, callback, [userContext])](/javascript/api/outlook/office.mailbox?view=outlook-js-1.7&preserve-view=true#outlook-office-mailbox-makeewsrequestasync-member(1)) | **read/write mailbox** | Compose<br>Read | [1.1](../requirement-set-1.1/outlook-requirement-set-1.1.md) |
| [removeHandlerAsync(eventType, [options], [callback])](/javascript/api/outlook/office.mailbox?view=outlook-js-1.7&preserve-view=true#outlook-office-mailbox-removehandlerasync-member(1)) | **read item** | Compose<br>Read | [1.5](../requirement-set-1.5/outlook-requirement-set-1.5.md) |

## Events

You can subscribe to and unsubscribe from the following events using [addHandlerAsync](/javascript/api/outlook/office.mailbox?view=outlook-js-1.7&preserve-view=true#outlook-office-mailbox-addhandlerasync-member(1)) and [removeHandlerAsync](/javascript/api/outlook/office.mailbox?view=outlook-js-1.7&preserve-view=true#outlook-office-mailbox-removehandlerasync-member(1)) respectively.

> [!IMPORTANT]
> Events are only available with task pane implementation.

| [Event](/javascript/api/office/office.eventtype?view=outlook-js-1.7&preserve-view=true) | Description | Minimum<br>requirement set |
|---|---|:---:|
|`ItemChanged`| A different Outlook item is selected for viewing while the task pane is pinned. | [1.5](../requirement-set-1.5/outlook-requirement-set-1.5.md) |
