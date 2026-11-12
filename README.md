# BiblioCrossing

This tool verifies bibliographic consistency in APA 7th edition documents. It cross-checks every
in-text citation against the reference list (and vice versa), flagging two common errors:
references listed but never cited in the text, and citations that appear in the text but are
missing from the reference list. Designed for editorial review of academic manuscripts, theses,
and journal articles.

**Use it:** https://alexescazu24-ship-it.github.io/apa7-citation-crossing/

Everything runs in the browser. The manuscript is never uploaded to any server, and no account or
installation is required.

---

## What it reports

Four are errors to fix, four are notices that do not always mean something is wrong.

| Label | Meaning |
|---|---|
| Citation without reference | Cited in the text, absent from the list |
| Uncited reference | In the list, never cited |
| Possible match | Same author, different year — usually a typo on one of the two sides |
| Duplicate reference | The same entry appears twice |
| Missing comma | `(García 2020)` instead of `(García, 2020)` — the citation is still cross-checked |
| Ambiguous surname | Two different authors share a surname and year; APA 7 asks for the initial in text |
| Personal communication | Cited in text only; APA 7 gives it no reference entry |
| Needs manual check | Laws, decrees and classical works use a different APA 7 reference format |

Secondary citations (`as cited in` / `como se citó en`) are resolved using the citing source, which
is the work that belongs in the reference list.

## Scope

Works with any manuscript that uses **author–date** citations and has a **reference section with a
heading**, in Spanish or English. It does not work with numeric styles (Vancouver, IEEE), footnote
styles, or documents without a reference section.

Input is a full manuscript — pasted text or a `.docx` file up to 10 MB. Legacy `.doc`, PDF and ODT
are not supported: convert to `.docx` or paste the text.

A built-in manual (📖 Manual in the header) documents every case in Spanish and English.

## Cite it

If you use this tool in published work, cite it with the metadata in
[`CITATION.cff`](CITATION.cff).

## Licence

- **Code:** [AGPL-3.0-or-later](https://www.gnu.org/licenses/agpl-3.0.html) — see [LICENSE](LICENSE)
- **Content and documentation:** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)
- The **BiblioCrossing logo and name** are reserved and covered by neither licence.
- The **Universidad Estatal a Distancia and Open Science Unit logos** are institutional
  trademarks, used here because the tool is the institution's own work, and they are
  **not covered by the licences above** either: reusing the code or the content gives no
  right to reuse those marks.

Copyright (C) 2026 Freddy Alexander Chinchilla Serrano, Carolina Seas, Steven Segura Jiménez

## Credits

Developed at the **Open Science Unit**, Vice-Rectory for Research, Universidad Estatal a
Distancia (UNED) · San José, Costa Rica · 2026

| Author | ORCID | Contribution |
|---|---|---|
| Freddy Alexander Chinchilla Serrano | [0000-0001-9465-1522](https://orcid.org/0000-0001-9465-1522) | Original idea, development |
| Carolina Seas | [0000-0002-2102-1973](https://orcid.org/0000-0002-2102-1973) | Development, improvements, testing |
| Steven Segura Jiménez | [0009-0005-6475-8798](https://orcid.org/0009-0005-6475-8798) | Development, improvements, testing |

Contact: fchinchillas@uned.ac.cr

**Coding:** Claude Code (Anthropic) — model identifier `claude-opus-5` — under human
editorial instruction, judgement and experience.
