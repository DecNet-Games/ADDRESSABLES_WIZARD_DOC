---
layout: default
title: Architecture
nav_order: 5
has_children: true
---

# 🏗️ Technical Architecture

Addressables Wizard is a strictly **Editor-Only** asset. 

---

## ⚡ Assembly Definition (ASMDEF)
The core logic resides within `DeoDevs.AddressablesSimplified.Editor.asmdef`.
- **Scope**: Editor-Only.
- **Platform**: Any platform supported by Unity.
- **Safety**: Logic is gated via *Version Defines* for the Addressables package.

## 📁 Folder Structure
```
Assets/DeoDevs/AddressablesSimplified
 ├─ Documentation/
 ├─ Editor/         # The Wizard, Analyzer, and Wrapper
 ├─ Runtime/        # Optional demo loaders
 └─ Demo/           # Example assets
```

> [!NOTE]
> All core logic is housed inside the `Editor` folder. It has **0% impact** on your game's runtime memory or CPU usage.

---

## 🔗 How It Works
1. When you click **Finish** in the Wizard, it generates `AddressableAssetSettings` assets in your project root.
2. It then configures **Profiles** (Local/Remote) via the `AddressablesAPIWrapper`.
3. Finally, it uses the **Asset Analyzer** to index and group your resources.

[Wrapper System ➔]({{ site.baseurl }}/docs/technical/wrapper-system.html)
