**CCBA Copilot Prompt Practice: update spec v2 (9 October 2026)**

**Task for the coding agent (paste this into the GitHub issue or Scout)**

Update index.html in jeffreysonola/ccba-copilot-prompt-practice to match this spec. Read prompts.json in this pack for every prompt; copy prompt text exactly, character for character, including line breaks and brackets. Open one pull request. Do not merge.

**Guardrails**

1. Never reword, shorten or 'improve' any prompt text. prompts.json is the only source of prompt wording.
2. Do not change existing exercises except where this spec says to move them.
3. Keep the current CCBA branding, colours, logo, theme handling and mobile layout.
4. Every new prompt gets the same copy control as the existing prompts. C2 is an instruction, not a prompt: no copy button.
5. Show each item's 'feature' as the capability callout and 'participant_tip' as the how-to line, using the existing exercise styling.
6. Do not add presenter-only content: no CDX names (Sydney, Amber, Mario), no mobile demo prompts, no Cowork prompts.
7. B3 links to the public PDF by URL. Do not commit the PDF to the repo.
8. Do not use em dashes in any new text.

**Target order of the site after the update**

1. Start Here: existing, unchanged
2. 1. Work IQ in four levels (B1 to B4): new; place directly after Start Here
3. 2. Your daily executive scan (C1, C2): new
4. 3. Make it yours (C3 to C7): replaces Exercise 0 layout; C5 is the existing 'Create personalized Copilot instructions' prompt and example, unchanged
5. 4. Prompt Coach (C8): new
6. 5. Researcher (R1, R2): existing Exercise 7, unchanged text, moved up
7. 6. Word: prepare for a business review: existing Exercise 3, unchanged; add a Legal Agent sub-section after it (see change 6)
8. 7. Excel: variance analysis: existing Exercise 4, unchanged; fix the download (see change 8)
9. 8. PowerPoint: build the Q3 business review: existing Exercise 5, unchanged
10. 9. Outlook: summarise, reply fast and sound like me: existing Exercise 6, unchanged
11. 10. More prompts to try (C13, C14): new, optional
12. 11. Your role (RS1 to RS6): new final exercise

Existing Exercise 1 (Prepare my day) and Exercise 2 (sugar-tax research) are not in the live run of show. Jeff decides whether to keep them as optional or hide them.

**Changes**

1. **Add 'Work IQ in four levels' (B1 to B4).** Intro line: 'The same Work IQ, four levels of prompting. Each level adds a little more to the prompt and one more Copilot feature.' Run all four in one conversation. B3 needs two link buttons:
   - Coca-Cola HBC 2026 Half Year Results Presentation (PDF): https://www.coca-colahellenic.com/content/dam/cch/us/documents/investors-and-financial/2026-half-year-results/coca-cola-hbc-2026-half-year-results-presentation.pdf.downloadasset.pdf
   - Coca-Cola HBC 2026 Half Year Results announcement: https://www.coca-colahellenic.com/en/media/news/financial_news/2026/2026-half-year-results
2. **Add 'Your daily executive scan' (C1, C2).** C1 is a prompt; C2 is a step with no copy button.
3. **Rebuild 'Make it yours' (C3 to C7).** Order: C3 Chief of Staff custom instructions, C4 shortcut test, C5 existing personalization prompt and example (unchanged), C6 Memory, C7 private reflection. C3 tip tells people to paste it into Settings > Personalization > Custom instructions.
4. **Add 'Prompt Coach' (C8)** with the worked example prompt from prompts.json.
5. **Move Researcher (existing Exercise 7) to sit after Prompt Coach.** No text changes.
6. **Legal Agent sub-section after Word.** Jeff adds his own Legal Agent prompts and document. The agent must not invent legal prompts: leave a clearly marked placeholder if Jeff has not supplied them.
7. **Add 'More prompts to try' (C13, C14)**, marked optional.
8. **Fix the Excel download.** CCBA_Q3_2026_Sales_Revenue_Tracker.xlsx returns an error instead of downloading. Check: (a) the href matches the filename and capitalisation exactly (GitHub Pages is case-sensitive); (b) the file is not a Git LFS pointer (a pointer is a ~130-byte text file); (c) the committed file opens in Excel locally; (d) the link has the download attribute and a relative path. Re-commit the real file if needed. Track this as a separate issue so the content update is not blocked.
9. **Add 'Your role' as the final exercise (RS1 to RS6).** Intro line: 'Pick the template closest to your role and run it on a real initiative, inserting your own document, deck, meeting or email with /.' Show each card with the role name, the persona line (from participant_tip) and the full prompt. Use only these six roles (CEO, CFO, COO, CHRO, CAO, CIO/CTO); the guide's other four roles are intentionally left out. RS1 changes the guide's '(board, donors, staff, beneficiaries)' to '(board, shareholders, staff, customers)'.

**Acceptance checks**

1. Every item in prompts.json appears once, in the order above, and its copied text equals the prompts.json 'prompt' value exactly.
2. Existing prompts for Word, Excel, PowerPoint, Outlook, Researcher and personalization are byte-for-byte unchanged.
3. Both B3 links open the Coca-Cola HBC pages; the Word and Excel exercise files both download and open.
4. Layout works at phone width and desktop width, in light and dark themes.
5. No CDX persona names, mobile demo prompts or Cowork prompts appear on the site.

**Files in this pack**

1. CHANGES-v2.md: this spec.
2. prompts.json: every participant-facing prompt with id, section, title, feature, participant_tip, files and status.
3. CCBA - Executive Copilot Session 9 Oct 2026 - Prompt Workbook.xlsx (shared separately): full context, including presenter prompts, run of show and CDX seeding. Use its 'Participant prompt (copy and adapt)' column if anything in prompts.json looks wrong.
