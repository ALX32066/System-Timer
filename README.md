<div align="center">

<img src="https://www.image2url.com/r2/default/images/1783883541864-bb22155b-96c9-47d2-8f3d-a66020f75b87.png" alt="System Timer Logo" width="150" height="150"/>

# ⏱️ System Timer

### An unbypassable, automated background workstation management utility developed by **A.L.X.**

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=20&pause=1000&color=1F6AA5&center=true&vCenter=true&width=560&lines=Invisible+Background+Enforcement;Unbypassable+Root-Level+Shutdown;Built+with+Python+%2B+CustomTkinter" alt="Typing SVG" />

<br/>

<img src="https://img.shields.io/badge/Platform-Windows%2010%20%7C%2011-blue?style=for-the-badge&logo=windows" alt="Platform"/>
<img src="https://img.shields.io/badge/Language-Python%203.x-yellow?style=for-the-badge&logo=python" alt="Language"/>
<img src="https://img.shields.io/badge/UI%20Framework-CustomTkinter-darkblue?style=for-the-badge" alt="Framework"/>
<img src="https://img.shields.io/badge/Developer-A.L.X.-orange?style=for-the-badge" alt="Developer"/>

<br/>

<img src="https://img.shields.io/badge/Status-Active-brightgreen?style=flat-square"/>
<img src="https://img.shields.io/badge/License-Proprietary-red?style=flat-square"/>
<img src="https://img.shields.io/badge/Version-1.0.0-blueviolet?style=flat-square"/>

</div>

---

## 📌 Project Overview

**System Timer** is a specialized production-security utility designed to enforce time management protocols directly at the OS level. It runs completely hidden in the background, allowing users to pre-define screen-time limits. Once deployed, the enforcement logic uses administrative rights to block standard user bypass strategies, ensuring the workstation safely commits and shuts down when thresholds are met.

<div align="center">

```
┌──────────────────────────────────────────────┐
│   BOOT → MONITOR → LOCK → WARN → SHUTDOWN     │
└──────────────────────────────────────────────┘
```

</div>

---

## 🚀 Key Features

<table>
<tr>
<td width="50%" valign="top">

### 🕵️ Invisible Background Execution
Operates seamlessly behind the scenes without distracting system tray icons or taskbar elements.

### 🔒 Grace Window & Secure Lockout
Allows full configuration adjustments within the first **30 minutes** of system boot. Afterward, the controls lock permanently until the next restart.

</td>
<td width="50%" valign="top">

### ⚡ Unbypassable Root Shutdown
Employs forced Windows shell execution (`shutdown /s /f /t 0`) preventing termination via conventional Task Manager operations.

### ⚠️ Prompt Warning Notification
Displays a high-visibility, closeable countdown overlay exactly **3 minutes** before shutdown, giving users time to save valuable progress.

</td>
</tr>
<tr>
<td colspan="2" valign="top">

### 📦 Native OS Packaging
Features a streamlined `.exe` bundle alongside an automated **Inno Setup** compiler for clean installations and full system uninstalls.

</td>
</tr>
</table>

---

## 🛠️ Architecture & Flow

```mermaid
graph TD
    A[💻 System Boot] --> B[🕵️ Invisible Background Service]
    B --> C{⌚ Time Check}
    C -->|First 30 Mins| D[🟢 Settings Editable]
    C -->|Post 30 Mins| E[🔴 Settings Locked]
    E --> F[⚠️ T-Minus 3 Mins: Warning Popup]
    F --> G[⚡ Timer Expiry: Enforced Hard Shutdown]

    %% CSS Styling for Colors
    style A fill:#2b2b2b,stroke:#888,stroke-width:2px,color:#fff
    style B fill:#1F6AA5,stroke:#fff,stroke-width:1px,color:#fff
    style C fill:#333,stroke:#1F6AA5,stroke-width:2px,color:#fff
    style D fill:#1b4d3e,stroke:#2ecc71,stroke-width:2px,color:#fff
    style E fill:#4d1b1b,stroke:#e74c3c,stroke-width:2px,color:#fff
    style F fill:#5e3a00,stroke:#f39c12,stroke-width:2px,color:#fff
    style G fill:#780000,stroke:#ff0000,stroke-width:2px,color:#fff
```

---

## ⚙️ Built With

<div align="center">

<img src="https://img.shields.io/badge/Python-3.x-3776AB?style=flat-square&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/CustomTkinter-GUI-1F6AA5?style=flat-square"/>
<img src="https://img.shields.io/badge/PyInstaller-Compiler-FFD43B?style=flat-square"/>
<img src="https://img.shields.io/badge/Inno%20Setup-Installer-6DB33F?style=flat-square"/>

</div>

| Component | Purpose |
|---|---|
| **Python 3.x** | Core logical service execution |
| **CustomTkinter** | Modern, premium dark-blue themed GUI components |
| **PyInstaller** | Compilation framework for cross-platform binary deployment |
| **Inno Setup Compiler** | Deployment automation script creating complete startup shortcuts and registry hooks |

---

## 💾 Installation & Setup

### ✅ Prerequisites
Ensure you have Windows 10/11 with local Administrator privileges.

### 🧩 Standard Deployment (Recommended)

1. Download the latest `System_Timer_Setup.exe` from the **Releases** tab.
2. Run the setup wizard (Fully branded by **A.L.X.** including licensing data).
3. The application will immediately bind to your `shell:startup` sequence.

### 🧑‍💻 Local Development Setup

If you plan to test or run the source files directly:

```bash
# Clone the repository
git clone https://github.com/your-username/System-Timer.git

# Navigate into the project directory
cd System-Timer

# Install dependencies
pip install customtkinter

# Run the app structure
python app.pyw
```

To compile your own executable with custom graphical icons:

```bash
pip install pyinstaller
pyinstaller --noconsole --onefile --icon=app_icon.ico app.pyw
```

---

## 🎯 How It Works (User Guide)

<table>
<tr>
<td width="33%" align="center">

**🔍 Accessing the App**

Because the window hides on launch, tap the `Windows Key` and search for **"System Timer"** to reveal the GUI dashboard.

</td>
<td width="33%" align="center">

**🎛️ Setting the Constraint**

Use the professional slider layout to shift runtime parameters (ranging from 35 to 180 minutes). Click **Save Settings**.

</td>
<td width="33%" align="center">

**🗑️ Safe Removal**

If you wish to suspend the service, simply uninstall it natively via `Apps > Installed Apps`. The uninstaller instantly flushes out background registries and shortcuts.

</td>
</tr>
</table>

---

## 📜 License & Copyright

<div align="center">

**Copyright (c) 2026 A.L.X. All Rights Reserved.**

<img src="https://img.shields.io/badge/©-2026%20A.L.X.-lightgrey?style=flat-square"/>

</div>
