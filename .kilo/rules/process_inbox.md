# PoE 2 Second Brain - Global Operating Rules

## ENVIRONMENT MANDATES
- ALL shell-related tasks (moving files, creating directories, deleting) MUST use **PowerShell** syntax.
- Documentation standard is **English** only.

## DATA PROCESSING WORKFLOW (Process Inbox)
When a user asks to "Process Inbox" or "Clean up", execute these steps:

1. **Pre-requisite**: 
    - Read `Vault_Guide.md` to understand the specific purpose and logic of each directory.
    - Reference this guide before making any movement decisions.

2. **Gather**: 
    - Read `00_Inbox/Quick_Notes.md`.
    - List all files in `00_Inbox/Unsorted/`.

3. **Analyze & Identify**: 
    - Identify technical PoE 2 mechanics, stats, and builds. 
    - Cross-check with directory rules from `Vault_Guide.md`.

4. **Naming & Identity Priority (Anti-Collision)**: 
    - **Source of Truth**: Existing manual notes and established vault names are priority.
    - **Transcript Handling**: Treat non-transcript names as superior. Speech-to-text (transcripts) can be inaccurate.
    - **Strict Rule**: Do not rename established entities or files back and forth based on transcript input.

5. **Distribute**: 
    - Move content to folders 01-06.
    - Use `01_Builds/Concepts/Build_Template.md` for new build discovery.

6. **Sync & Link**:
    - Search vault for consistency.
    - Update master files if new info adds value, but **preserve unique proper names**.
    - ALWAYS create `[[Wiki Links]]` for cross-referencing.

7. **Mark Uncertainty**: Use `??` or `#unconfirmed` for speculative data.

## CLEANUP PROTOCOL
- Only delete files in `00_Inbox/Unsorted/` AFTER they have been successfully summarized or moved.
- When clearing `00_Inbox/Quick_Notes.md`, keep the top header/title.

## SAFETY
- Ask for confirmation before mass-deleting more than 5 files.