# Power-Automate-Desktop-Folder-Organizer
# 📂 Power Automate Desktop: Automated Folder Organizer

A beginner-friendly Low-Code/No-Code automation script built using **Power Automate for Desktop**. This bot automatically scans a designated messy folder (like the Downloads directory), isolates specific file types (such as Excel sheets), and organizes them into a clean, newly created destination folder.

---

## Project Overview
* **Goal**: Eliminate manual file filing and desktop clutter.
* **Tool Used**: Power Automate for Desktop
* **Target Environment**: Windows Local OS
* **Core Logic**: Input (Scan Folder) ➡️ Process (Filter by `.xlsx`) ➡️ Action (Create Directory & Move Files)

---

## How It Works (Step-by-Step Logic)

The automation follows a simple 3-step sequence:

1. **Get Files in Folder**: Scans the source directory (`%Downloads%`) using a file filter limit of `*.xlsx` to target only Excel spreadsheets.
2. **Create Folder**: Dynamically generates a brand new folder named `Organized Excel Files` on the desktop if it does not already exist.
3. **Move Files**: Transfers the gathered array list of Excel files from the source path directly into the newly created target directory, overwriting any duplicates to avoid system halts.

---

## How to Use This Flow
1. Install **Power Automate for Desktop** on a Windows machine.
2. Create a **New Flow**.
3. Open the `flow_script.txt` file included in this repository.
4. Copy the entire block of text, then click inside the main center workspace of your Power Automate Designer window and press `Ctrl + V` (Paste). The visual actions will automatically generate!
5. Update the folder directory paths in Step 1 and Step 2 to match your personal PC paths, then click **Run**.
