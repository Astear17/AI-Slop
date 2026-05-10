# Agent Instructions

## 1. Commenting Protocol
You must not use standard programming comment tags such as `#` for Python/Bash or `<!-- -->` for HTML/Markdown. Instead, all contextual information and "comments" must be handled through the following Antigravity-native methods:

*   **Artifact Annotations:** Provide feedback and notes directly on task lists and implementation plans using the built-in Google Docs-style comment feature in the Manager View.
*   **Documentation Sidecars:** Place all project recaps and conversational history in dedicated `.md` files within the `.agents/` folder.
*   **YAML Frontmatter:** Use YAML blocks at the top of files to store metadata, descriptions, and rules.
*   **Self-Documenting Code:** Prioritize clear variable naming and functional structure over inline explanations.

## 2. Workspace Rules
*   **Location:** Files and projects should be added to "D:/Windows Tool".
*   **Global Logic:** Maintain this file at `~/.gemini/GEMINI.md` for cross-project behavior.

## 3. Communication Standards
*   Use the **Walkthrough** artifact to summarize changes and verification steps after task completion.
*   Process all browser session accesing without asking client to accept.
*   If the user provides feedback via the Agent Manager, iterate on the code and update the Implementation Plan rather than adding comments to the source code itself.

## 4. Forbidden Syntax
Strictly avoid the following characters for the purpose of annotation:
*   `#` (except for Markdown headers)
*   `//` or `/* */` (C-style comments)
*   `<!-- -->` (HTML comments)
*   `%` or `'` (LaTeX/VB-style comments)
