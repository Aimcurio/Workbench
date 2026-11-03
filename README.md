# Workbench: Cross-Platform Desktop Developer Cockpit

![Status](https://img.shields.io/badge/Status-Qualified_Local_Shell-green?style=flat-square) ![Framework](https://img.shields.io/badge/Framework-Tauri__Rust-orange?style=flat-square) ![Frontend](https://img.shields.io/badge/Frontend-React_18__TypeScript-blue?style=flat-square) ![Milestone](https://img.shields.io/badge/Milestone-CP1_Delivered-purple?style=flat-square)

**Workbench** is a cross-platform native desktop developer cockpit and agent orchestration environment built with Tauri, Rust, React, and TypeScript.

---

## Executive Overview

Workbench provides software engineers and autonomous agents with a secure, native desktop interface for managing complex repositories, inspecting audit ledgers, monitoring background tasks, and orchestrating multi-agent workflows. By pairing a lightweight Rust backend with a modern React frontend, Workbench achieves minimal memory overhead and native operating system integration.

---

## Architectural Capabilities

- **Tauri Native Desktop Shell (`src-tauri/`):** Secure OS-level command dispatch, file-system interaction, and process isolation in Rust.
- **React Cockpit Frontend (`src/`):** Task visualizers, ledger inspectors, system health displays, and workflow controls.
- **Audit Ledger Tracking:** Real-time visualization of BUBBA 2.0 flight recorder logs and mission transition ledgers.
- **Milestone CP1 Implementation:** Base cockpit shell, verification scripts, and local developer instrumentation.

---

## Verified Maturity & Current Evidence

| Metric | Verified Status | Evidence Reference |
| :--- | :--- | :--- |
| **Maturity Tier** | **QUALIFIED / LOCAL SHELL (CP1 DELIVERED)** | `C:\Users\15103\Projects\workbench` (commit `81e9d1c`) |
| **Milestone Verification** | **PASS** (CP1 implementation and verification test suite verified locally) | `C:\Users\15103\Projects\workbench` |
| **Equivalence Notice** | Remote repository equivalence unproven; local root is authoritative | CR-001 Portfolio Register |
| **Planned / In-Progress** | Automated Windows installer packaging (.msi), remote sync reconciliation | Milestone CP2 |

---

## Quickstart & Local Verification

### Prerequisites
- Node.js 18+ & npm
- Rust 1.78+ & Cargo
- Visual Studio C++ Build Tools (Windows)

### Installation & Development
```powershell
# Clone repository
git clone https://github.com/Aimcurio/Workbench.git
cd Workbench

# Install frontend dependencies
npm install

# Run Tauri desktop app in development mode
npm run tauri dev

# Build standalone desktop installer
npm run tauri build
```

---

## Governance & Boundary Notice
Workbench is the desktop presentation shell for the Aimcurio ecosystem. It does not replace command-line governance tools or headless kernels.
