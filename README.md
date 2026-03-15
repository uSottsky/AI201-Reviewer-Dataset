# AI201-Reviewer-Dataset

This repository contains an Obsidian note dataset for AI 201 (Artificial Intelligence) review materials. All notes, quizzes, and resources are formatted for use with Obsidian, including compatibility with quiz, flashcards and study plugins.

---

## Guide: Using This Dataset in Obsidian to Generate Anki Flashcards

### 1. Install Obsidian
- Download and install Obsidian from the [official website](https://obsidian.md/).
- Open Obsidian and set your vault to this dataset folder.

### 2. Install the Obsidian to Anki Integration Plugin
- In Obsidian, go to **Settings > Community plugins**.
- Search for and install the plugin: **Obsidian to Anki** (or similar, e.g., Obsidian Anki Bridge).
- Enable the plugin after installation.

### 3. Install Anki
- Download and install Anki from the [official website](https://apps.ankiweb.net/).
- Open Anki and set up your profile.

### 4. Install AnkiConnect (for integration)
- In Anki, go to **Tools > Add-ons > Get Add-ons**.
- Enter the code for **AnkiConnect** (usually `2055492159`).
- Restart Anki to activate the add-on.

### 5. Configure Obsidian to Export Flashcards to Anki
- In Obsidian, open the plugin settings for your Anki integration plugin.
- Set up the connection to Anki (ensure Anki is running with AnkiConnect enabled).
- Configure flashcard note types and decks as needed.

### 6. Formatting Flashcards in Markdown
- Use the following format in your markdown files for flashcards:
  ```
  ## Flashcard
  **Q:** What is the decision rule for classifying a pattern in a trained MLP?
  **A:** Assign the input vector $x$ to class $C_k$ if the corresponding output $F_k(x)$ is greater than or equal to $F_j(x)$ for all $j \ne k$.
  ```
- Or use the syntax required by your chosen plugin (e.g., `Question:: Answer` or `Q: ...\nA: ...`).

### 7. Exporting Flashcards to Anki
- Use the plugin command (e.g., "Export to Anki") in Obsidian to send your flashcards to Anki.
- Review and study your flashcards in Anki as usual.

---

For more details, refer to the documentation of the Obsidian plugin and AnkiConnect.