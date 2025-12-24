# Twisted Auto-Roller

A lightweight desktop tool for **Twisted** that monitors the in-game **Thermodynamics** panel, **OCR-parses key composite values**, and helps you quickly identify “good” servers. Includes a clean UI, analytics, and optional Discord webhook alerts.

> **Note:** This project reads the screen and sends in-game key sequences. Use responsibly and follow the game’s rules/community guidance.

---

## Features

- **Health-bar detection** (pixel search) to know when you’re fully loaded
- Opens **Thermodynamics** and uses **Tesseract OCR** to parse:
  - **STP**
  - **VTP**
  - **CAPE**
  - **SRH**
- **Filter rules** (comparators + thresholds) to define what “good” means
- **Good Server Found** popup:
  - Shows STP/VTP/CAPE/SRH
  - Buttons to **Continue rerolling** or **Stop rolling**
  - Always-on-top popup (can appear over Roblox)
- **Analytics tab**:
  - Highest/Lowest rolled values (STP/VTP/CAPE/SRH)
  - Session history table (most recent first)
- **Discord webhook support** (optional):
  - Purple-styled embed
  - Optional **User ID ping**
  - Includes a server link in alerts (when available)
- Stores config/logs in a local data folder (no external database)

---

## Requirements

### Windows
- Python 3.10+ recommended
- Roblox (or Bloxstrap, optional)
- **Tesseract OCR** installed
