---
title: OfficeTab element in the manifest file
description: The OfficeTab element defines the ribbon tab where your add-in command appears.
ms.date: 08/01/2023
ms.localizationpriority: medium
---

# OfficeTab element

Defines the built-in Office ribbon tab on which your add-in command appears. If you want the add-in command to appear on a custom tab of your own, use the [CustomTab](customtab.md) element.

**Add-in type:** Task pane, Mail

**Valid only in these VersionOverrides schemas**:

- Taskpane 1.0
- Mail 1.0
- Mail 1.1

For more information, see [Version overrides in the manifest](/office/dev/add-ins/develop/add-in-manifests#version-overrides-in-the-manifest).

**Associated with these requirement sets**:

- [AddinCommands 1.1](../requirement-sets/common/add-in-commands-requirement-sets.md) when the parent **\<VersionOverrides\>** is type Taskpane 1.0.
- [Mailbox 1.3](../requirement-sets/outlook/requirement-set-1.3/outlook-requirement-set-1.3.md) when the parent **\<VersionOverrides\>** is type Mail 1.0.
- [Mailbox 1.5](../requirement-sets/outlook/requirement-set-1.5/outlook-requirement-set-1.5.md) when the parent **\<VersionOverrides\>** is type Mail 1.1.

## Child elements

|  Element |  Required  |  Description  |
|:-----|:-----:|:-----|
|  Group      | Yes |  Defines a group of commands. You can add only one group per add-in to the default tab.  |

The following are valid tab `id` values by application. Values in **bold** are supported in both desktop and online (for example, Word 2016 or later on Windows and Word on the web).

### Outlook

- **TabDefault** (either **Home**, **Message**, or **Meeting**)

### Word

- **TabHome**
- **TabInsert**
- **TabWordDesign**
- **TabPageLayoutWord**
- **TabReferences**
- **TabMailings**
- **TabReviewWord**
- **TabView**
- **TabDeveloper**
- **TabAddIns**
- TabBlogPost
- TabBlogInsert
- TabPrintPreview
- TabOutlining
- TabConflicts
- TabBackgroundRemoval
- TabBroadcastPresentation

### Excel

- **TabHome**
- **TabInsert**
- **TabPageLayoutExcel**
- **TabFormulas**
- **TabData**
- **TabReview**
- **TabView**
- **TabDeveloper**
- **TabAddIns**
- TabPrintPreview
- TabBackgroundRemoval

### PowerPoint

- **TabHome**
- **TabInsert**
- **TabDesign**
- **TabTransitions**
- **TabAnimations**
- **TabSlideShow**
- **TabReview**
- **TabView**
- **TabDeveloper**
- **TabAddIns**
- TabPrintPreview
- TabMerge
- TabGrayscale
- TabBlackAndWhite
- TabBroadcastPresentation
- TabSlideMaster
- TabHandoutMaster
- TabNotesMaster
- TabBackgroundRemoval
- TabSlideMasterHome

### OneNote

- **TabHome**
- **TabInsert**
- **TabView**
- TabDeveloper
- TabAddIns

## Group

A group of UI extension points in a tab. A group can have up to six controls. The **id** attribute is required and each **id** must be unique among all groups in the manifest. The **id** is a string with a maximum of 125 characters. See [Group element](group.md).

## OfficeTab example

```xml
<ExtensionPoint xsi:type="MessageReadCommandSurface">
  <OfficeTab id="TabDefault">
    <Group id="Contoso.msgreadTabMessage.group1">
        <!-- Group Definition -->
    </Group>
  </OfficeTab>
</ExtensionPoint>
```
