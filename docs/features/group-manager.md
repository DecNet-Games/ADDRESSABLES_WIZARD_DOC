---
layout: default
title: Group Manager
parent: Features
nav_order: 2
---

# 📦 Group Manager

A specialized alternative to Unity's native Groups window, focused on organization and speed.

---

## ⏩ Mark Folder Shortcut
The **Mark Folder** button is the Wizard's most powerful feature.
1. Enter the group name (e.g., `Enemies`).
2. Specify the asset folder (e.g., `Assets/Art/Characters/Enemies`).
3. Click **Index**.

The Wizard will:
- Check every asset in the folder.
- Add it to the Addressables group.
- **Safety**: Move assets back to the default group if the original group is deleted, preventing resource loss.

---

## 📊 Group Summaries
Each group entry in our manager provides:
- **Asset Count**: Total number of individual resources tracked.
- **Toggle State**: One-click enable/disable.
- **Delete Group**: Safely removes the category and re-assigns its assets.

> ### 💡 Pro Tip
> Use the **Mark Addressable** context menu (Right-Click in Project view) to instantly add assets on the fly.
