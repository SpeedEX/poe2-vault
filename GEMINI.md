# PoE 2 Vault: Agent Instructions

This file provides foundational mandates for any AI agent interacting with this workspace. Adhere strictly to these guidelines to maintain the integrity and organization of the "Second Brain."

## 🛠️ Environment & Command Mandates

- **Environment Detection**: At the start of every session or when executing shell commands, verify the current operating system (e.g., `win32`) and terminal (e.g., PowerShell).
- **Command Syntax**: 
    - On Windows, strictly use **PowerShell** syntax. 
    - Avoid using bash-specific flags (e.g., `ls -a`) unless explicitly supported. 
    - Use PowerShell equivalents like `Get-ChildItem -Force` or `Test-Path`.
- **Validation**: If a command fails due to environment mismatch, immediately correct the strategy to use the native shell of the current system.

## 📂 Information Management Workflow

All information processing must follow these four steps:

1.  **Capture**: Place raw info or quick thoughts into the `00_Inbox/`.
2.  **Process**: Analyze whether the data belongs to a Build, System, Item, or Map category.
3.  **Store**: Summarize data into Markdown format and move it to the appropriate directory (`01-06`).
4.  **Link**: Create cross-references (wikilinks `[[filename]]`) between files to build a cohesive knowledge graph.

## 🏗️ Core Directory Mandates

- **Builds (`01_Builds/`)**: Always use `01_Builds/Concepts/Build_Template.md` when generating new character builds.
- **Systems (`02_Systems/`)**: Store mechanics knowledge here. Refer to `Patch_Notes_0.5_Summary.md` for current game version context.
- **Assets (`03_Assets/`)**: Keep crafting recipes and unique item data synchronized with the latest community findings.
- **Campaign (`06_Campaign/`)**: Ensure `Permanent_Buffs.md` is updated whenever a leveling walkthrough is processed.

## 📝 Style & Formatting

- Use **Obsidian-style wikilinks** (`[[Link]]`) for internal referencing.
- Maintain a professional, technical tone suitable for a "Second Brain."
- Prefer concise Markdown headers and bulleted lists for readability.

## 🤖 Interaction Preferences

- When asked to "process the inbox" look for files in `00_Inbox/Unsorted/` and suggest where they should be moved/summarized.
- When asked to "process my quick notes" read `00_Inbox/Quick_Notes.md`, distribute the information to appropriate vault files, and then clear the content of `Quick_Notes.md` (preserving the header).
- Always check `Vault_Guide.md` if the purpose of a directory is unclear.

## ❓ Handling Uncertainty

- If a note or fragment contains markers like `??`, `TODO`, or `#unconfirmed`, explicitly mark these as **Speculative** or add them to a **To Do** list in the final document.
- Never assume unconfirmed gameplay theories are facts; always preserve the user's original doubt in the summarized version.
