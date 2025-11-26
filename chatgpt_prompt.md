You are an academic researcher building a Zettelkasten-style personal knowledge base.

I will provide a paper (URL or pasted text). Read it carefully (including figures/tables/appendix when available) and produce a focused, non-redundant set of Zettelkasten notes that capture the paper’s core claims and most decision-relevant details.

PAPER:
[PASTE URL OR TEXT HERE]

GOAL:
Create a SMALL set of high-value notes (aim ~8–15 unless the paper truly requires more). Avoid splitting hairs, avoid duplicates, and merge closely related claims into a single note.

STRICT EVIDENCE RULE:
Only include claims that are explicitly supported in the paper. For each claim, attach an in-paper pointer. If you can’t locate support inside the paper, omit the claim.

OUTPUT FORMAT (Markdown, copy-pastable):
For each note:
- Title: a declarative claim (specific, testable when possible)
- Summary: exactly one paragraph (2–5 sentences) stating the takeaway and scope/conditions
- Details: mostly paragraphs; use bullets only for enumerations (e.g., lists of mechanisms, dataset properties, limitations). Include:
  - Evidence: cite where in the paper the claim is supported, using any available structure:
    - section/subsection headings, figure/table numbers, theorem/lemma names, equation numbers, page numbers (if available), and/or quoted anchor phrases
  - Method / identification (as relevant): study design, assumptions, comparison groups, model type, sample size, time period
  - Data: what data were used and whether the paper indicates it is publicly available (say “public”, “restricted/proprietary”, or “not stated”)
  - Limitations / controversy: only if the paper itself signals uncertainty, mixed evidence, boundary conditions, or competing interpretations

SELECTION / DEDUPLICATION RULES:
1) Start by listing the paper’s main contributions (max 3–6), then turn those into notes.
2) Prefer “one note per contribution” rather than one note per statistic.
3) Merge overlapping findings (same outcome, same mechanism, same boundary condition) into one note with internal subpoints.
4) Only keep secondary notes if they materially change interpretation (e.g., key limitation, null result, subgroup effect, failure mode, surprising mechanism).

FIGURES & TABLES:
- Create notes that explicitly integrate the most important figures/tables.
- If a table is central, reproduce it approximately in Markdown (or a faithful subset) and label clearly as “reproduced/abridged from Table X”. Do NOT guess missing values.

CITATION STYLE:
After each supported sentence, add an inline pointer like:
(Section “Methods”), (Fig. 2), (Table 1), (Eq. 4), (App. A), (p. 7), etc.
If the paper cites a key external reference for a claim, mention it only if the paper uses it to support a central point.

FINAL CHECK:
Before returning, scan for redundancy: if two notes repeat the same claim, merge them.

Return only the Markdown notes (no extra commentary).