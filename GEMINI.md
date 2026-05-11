# PoE 2 Vault: Agent Instructions (Gemini 3 Optimized)

This file provides foundational mandates for any AI agent interacting with this workspace.

## Environment & Commands
- **Shell**: Strictly **PowerShell** (win32). Use `Get-ChildItem`, `Move-Item`, `Test-Path`.
- **Validation**: Check destination existence before moving. On failure, analyze error and retry.

## Data Integrity & Naming (CRITICAL)
- **Authority**: Existing files in `01-06` are the primary source of truth.
- **Naming Priority**: **STRICTLY PRESERVE** established entity names. Do not "correct" names based on transcript errors (e.g., if vault has "Mageblood", ignore transcript saying "Mage Blud").
- **Deduplicate**: ALWAYS `search_files` before creating new ones to prevent redundant clones.
- **Link**: Use Obsidian-style `[[Wiki Links]]` for all internal references.

## Directory Mandates
- 01_Builds: Mandatory use of 01_Builds/Concepts/Build_Template.md for new builds.
- 02_Systems: Reference Patch_Notes_0.5_Summary.md for version context.
- 06_Campaign: Update Permanent_Buffs.md immediately if quest rewards are identified.
- General: For directory purposes not listed here, strictly follow Vault_Guide.md.

## Interaction & Style
- **Tone**: Professional, technical, English only. No conversational filler.
- **Cleanup**: (When triggered by commands) Clear `Quick_Notes.md` body (keep header) and delete processed `Unsorted/` files.
- **Visuals**: Bold key PoE 2 stats/mechanics (e.g., **Spirit**, **Cast Speed**) for readability.

## Uncertainty
- **Speculative**: Mark `??` or `#unconfirmed` as **[SPECULATIVE]**.
- **Gaps**: Use `ask_followup_question` if critical info is missing to complete a task.