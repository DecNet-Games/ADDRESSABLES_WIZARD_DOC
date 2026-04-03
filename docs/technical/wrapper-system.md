---
layout: default
title: Wrapper System
parent: Architecture
nav_order: 1
---

# 🛡️ Wrapper System

Unity's `Addressables` and `AddressableAssetSettings` APIs are only available within specific namespaces and require a package reference. 

---

## 🔒 Safety Layer
The `AddressablesAPIWrapper.cs` is the core safety bridge between our tool and Unity's API. 
- **Method Scope**: Uses `#if ADDRESSABLES_PRESENT` blocks to gate all communication.
- **Why it matters**: If you uninstall the `Addressables` package, every single line of code in the Wizard remains valid and your project will **still compile**.

---

## ⚡ Non-Reflective Installation
While other tools use slow, error-prone Reflection to install packages, our `PackageInstaller.cs` uses the official asynchronous `PackageManager.Client` API.
- **Robustness**: Provides `PackageManager.Request` status (In Progress, Success, Failure).
- **Automation**: One-click installs and project-wide dependency resolution.

> [!IMPORTANT]
> The Wrapper System ensures that the Addressables Wizard is **0% impact** at runtime. Every script is stripped before your final build.
