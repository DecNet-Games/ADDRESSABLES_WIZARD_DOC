---
layout: default
title: Content Building
parent: Features
nav_order: 3
---

# 🔨 Content Building

The **🔨 Build** tab is your command center for asset distribution. 

---

## 🏗️ Building Your Content
When you hit **Build Addressables**, the Wizard will:
1. Verify the current build target (Android, iOS, PC, etc.).
2. Synchronize all groups and paths.
3. Call the Unity `AddressableAssetSettings.BuildPlayerContent()` method.
4. Update the **Dashboard** with the new build timestamp and storage path.

---

## 🧹 Clean Builds
If you're noticing strange loading behavior or corrupted assets:
- Use **Clean Addressables** to wipe the internal bundle cache.
- This ensures your next build is a 100% fresh compilation of your resources.

> [!WARNING]
> Cleanup is permanent for local caches. Use it when transitioning between large project version updates.
