# Lucent_Notes
Lecture structurer MVP

## Current Status: Active Pre-Coding Phase
*This repository was created on [2025-10-28] to publicly document the journey of building a note-structuring AI from the ground up. I am currently in the "Wizard of Oz" phase, manually processing notes to discover the core rules of structure.*

## The Goal
To transform messy, handwritten notes into clean, structured digital documents.

## The Structurer's Rulebook (In Progress)
These are the rules I've discovered by manually processing user notes. This list will grow as I learn.

### Rule 1: The Prime Directive - Preservation
**Never alter the user's original text.** The goal is to reorganize, not to rewrite. Changing a single word destroys trust. (Learned from: Polish note failure[2025-10-18]).

### Rule 2: Title Detection
A line is likely a **Title** if it is:
- Centered at the top of a section.
- Written with larger or bolder text.
- Underlined.
- Followed by a large empty space.

### Rule 3: List Detection
A line is likely a **List Item** if it starts with:
- A bullet point (`•`, `-`).
- A number followed by a period or parenthesis (`1.`, `1)`).
- A letter followed by a period or parenthesis (`a.`, `a)`).

### Rule 4: Context over Perfection
If a word is blurry, use the surrounding sentence to guess the word. Prioritize making the sentence make sense over perfect individual character recognition. (Learned from: Manually correcting AI OCR mistakes).

## Next Steps
1.  Process 5 more user note sets to find new rules and validate these.
2.  Begin building a simple Python script to automate the application of these rules to digital text.
