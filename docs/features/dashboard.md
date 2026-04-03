---
layout: default
title: Dashboard & Stats
parent: Features
nav_order: 1
---

# 📊 Dashboard & Stats

The **📊 Dashboard** provides a constant project "Heartbeat," giving you bird's-eye-view analytics without digging into sub-menus.

---

## 🔍 Key Analytics

### 1. Asset Marking Status
Instantly see which portions of your `Project` folder are marked as Addressables. The dashboard visualizes:
- **Total Marks**: How many individual assets are being tracked.
- **Group Distribution**: Percentage of assets per category.

### 2. Build Monitor
The **Last Successful Build** entry shows:
- **Timestamp**: Exactly when your bundles were compiled.
- **Storage Path**: Where your platform-specific bundles are currently stored.
- **Size Estimation**: The total uncompressed footprint of your addressable content.

---

## 🛡️ Health Auditing
The Dashboard uses the **Asset Analyzer** (Intelligence Layer) to alert you of potential build failures before they happen.
- **⚠️ Circular References**: Detects if `Asset A` depends on `Asset B`, and vice-versa, which could cause a build failure.
- **⚠️ Unused Bundles**: Highlights assets marked as Addressables but not referenced anywhere in your scenes.

> [!TIP]
> Use the **Quick Links** on the bottom of the Dashboard to jump between Profiles, Groups, and the Build tab.
