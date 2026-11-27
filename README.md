# Report Comment Builder

Build school report comments from **your own comment bank** and **your own markbook**.

**Use it here: https://sabrinahoang0.github.io/report-comment-builder/**

Everything runs in your web browser. Comment banks and markbooks are read on your own computer and kept in that browser only; nothing is uploaded to a server, so no student names or marks leave your device.

## What it does

- **One student:** choose a grade, the student's name and pronouns, and pick a sentence for each part of the comment (Opening, Participation, Progress, any extra parts, Reflection). The comment is assembled as you go, ready to copy or edit.
- **Markbook:** import an Excel or CSV markbook and it writes a comment for every student, using their grade, their strongest mark for Progress and their weakest mark for the Reflection. Review, edit any comment, then download the markbook with a comment column added, or copy the comments straight into your own markbook.
- **Checks:** repeated words are highlighted, and words that contradict each other (for example "diligent" and "distracted") are underlined in red.
- Options for students who are sometimes or often distracted, late submissions, absences and other add-on sentences.

## Comment bank format

Upload a **Word document (.docx)** or a **spreadsheet (.xlsx or .csv)**.

**Word:** give each part a heading (for example "1. Opening", "2. Participation", "3. Progress", "Optional add-ons", "4. Reflection") with a table under it. The last column of each table is the sentence; the columns before it are its label, such as the grade ("Outstanding (A)", "B", "C–D") and, for Progress, the area ("Speaking", "Writing"). Any other heading with a table (such as "Hiragana") becomes an extra part of the comment. Headings such as "How to use" and "Sample comments" are skipped.

**Without tables:** under each part's heading, put the grade as a subheading ("Outstanding (A)") with its sentences below it, or at the start of each line ("Outstanding (A): {first_name} is…", "B – {first_name} is…"). For Progress, add the area after the grade ("High (B) – Speaking: …") or as a smaller subheading. Lines without a `{field}` are treated as notes and left out. Give extra parts a heading style or a number ("4. Hiragana"). Plain text files (.txt or .md, with `#` headings) are read the same way.

**Spreadsheet:** one row per sentence with the columns **Part**, **Label**, **Area** (optional) and **Comment**. Download the template from the Comment banks tab for an example.

**In the sentences** use `{first_name}`, `{he_she}`, `{his_her}`, `{him_her}` and `{himself_herself}`. Put grades A to E in the labels so the right sentences are offered for each grade. Reflection labels starting "Weak" (for example "Weak writing") are used when that area is a student's lowest mark. Words in `[square brackets]` are left for you to fill in.

## Markbook format

One row per student. It needs a first-name column (or a "Surname, First name" column) and a grade column (A to E). Optional columns: pronoun or gender, a mark for each assessment area, a mark for any extra part of the comment such as Hiragana, distracted (sometimes / often) and late submission (yes). A mark for an extra part decides that part's sentence (85% or more gives the A sentence by default; the cut-offs can be changed) and, if it is at C level or below, its "Weak …" Reflection. The Markbook tab can download a blank template for the comment bank you're using.

## Credits

Word files are read with [mammoth.js](https://github.com/mwilliamson/mammoth.js) and spreadsheets with [SheetJS](https://sheetjs.com/); their licences are in the `vendor` folder.
