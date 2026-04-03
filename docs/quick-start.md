---
layout: default
title: Quick Start
nav_order: 3
---

# ⚡ Quick Start

The **Setup Wizard** is your starting point for any new project. It automates every single step of the Addressable system's initial configuration.

---

## ⚡ The 5-Minute Walkthrough

### 1. Launch the Wizard
Navigate to **Tools > DecNet > Addressables Wizard**. 
If you haven't configured your settings yet, the Wizard will open automatically.

### 2. Choose Your Strategy
- **Local Only**: For projects that bundle all assets within the final build.
- **Remote**: For live service games (e.g., assets on AWS/S3 or Azure).
- **Hybrid**: A mix of both for optimized performance.

### 3. Create Asset Groups
Define your categories:
- `Environments`
- `Characters`
- `UI_Main`

> [!TIP]
> Keep your groups focused. The Wizard will automatically create these in the background for you.

### 4. Mark Folders
Enter the folder paths of your assets (e.g., `Assets/Art/Characters`). 
The Wizard will bulk-mark every asset in those folders as an "Addressable" and assign them to the correct group.

### 5. Build Your First Bundle
Click **Finish**. The Wizard will generate all necessary profile settings, clean existing caches, and trigger your first content build.

---

## ✅ What Just Happened?
In under 60 seconds, you have:
- Installed the Unity Addressables package.
- Created Local/Remote load paths.
- Bulk-indexed your project resources.
- Compiled your first asset bundle for your current platform.

[Features Overview ➔]({{ site.baseurl }}/docs/features/dashboard.html)
