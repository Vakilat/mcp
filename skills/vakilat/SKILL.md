---
name: vakilat
description: Find and check Supreme Court of India authorities with the Vakilat tools. Use for any question about Indian law or legal work in India, such as a point of law, a section of an Act, a case name, a citation (SCC, AIR, SCR, SCC OnLine or INSC), a quotation from a judgment, a case number, or how an IPC, CrPC or Indian Evidence Act section maps to the BNS, BNSS or BSA. Also use when the user asks what Vakilat holds or what its tools can do.
---

# Vakilat

Vakilat's tools search and read the judgments of the Supreme Court of India from 1950, as the
Court published them in its official copies, with the Court's own paragraph numbers. They hold no
High Court or tribunal judgments yet, and no statute text beyond the table of old and new
criminal code sections.

## When a question is about Indian law or legal work in India

1. Find the authorities before answering:
   - a point of law, a provision, a judge or the parties' names: `search_judgments`;
   - a citation: `find_by_citation`; a case number: `find_by_case_number`;
   - a point inside one judgment: `search_within`;
   - an IPC, CrPC or Indian Evidence Act section and its BNS, BNSS or BSA counterpart, or back:
     `old_and_new_code`.
2. Read the paragraphs an answer relies on with `read_paragraphs`. Search snippets are excerpts
   for choosing what to read, not text to quote.
3. Check every citation and quotation the answer relies on with `check_citation`, including any
   the user supplies. Give the paragraph number when the quote names one.
4. For how a judgment was later treated, use `cited_by`, then read the citing paragraph. A
   judgment that cites another has not necessarily followed it. For what a judgment relied on,
   use `authorities_cited`.

## How to write the answer

- Quote only paragraph text a tool returned, word for word, with its paragraph number and the
  paragraph's Vakilat link.
- Never cite a judgment, citation or paragraph that no tool returned.
- When `check_citation` reports a quote is not word for word, do not present it as the Court's
  words. When it reports not_found or unverified, say so plainly.
- When the tools return no authority on a point, say plainly that Vakilat has none. For a
  citation Vakilat does not hold, that alone does not prove the citation wrong.
- Give the Vakilat or official link for every authority, and tell the reader to check it before
  relying on it.

## What Vakilat contains

- Supreme Court of India judgments from 1950, from the Court's official copies, with the Court's
  own paragraph numbers and page numbers.
- Word-for-word checks of a quotation against the judgment, and against a named paragraph.
- Later Supreme Court judgments that cite a judgment, with the citing paragraph. These are
  citations, not treatment labels: they do not say followed, distinguished or overruled.
- The authorities a judgment cites, as printed in it.
- The table of old and new criminal code sections: IPC to BNS, CrPC to BNSS and the Indian
  Evidence Act to the BSA, with links to the official text of both codes.
- No High Court or tribunal judgments yet.

The tools do not open the lawyer's Vakilat matters, documents or Library. Vakilat receives only
what each tool needs, such as a query, a citation or a quotation.

## Limits to state

- Vakilat is research help for lawyers, not legal advice. A qualified lawyer reviews any
  output before it is relied on for advice, a filing or any decision.
- Each Vakilat account has a daily number of tool calls per seat: 30 on the free plan, and 100,
  300 or 1,000 on the paid plans. When the limit is reached, the tool says so and says when it
  resets, at midnight India time.
