# Vakilat for AI assistants

Vakilat's tools let the AI assistant you already use search, read and check the judgments of
the Supreme Court of India. The assistant writes the answer; the tools give it the Court's own
words, paragraph numbers and links to check them.

This repository holds the Vakilat plugin: one skill, `skills/vakilat/SKILL.md`, that tells the
assistant when and how to use the tools, and the address of Vakilat's remote MCP server,
`https://api.vakilat.io/mcp`.

## What it contains

- Supreme Court of India judgments from 1950, from the Court's official copies, with the
  Court's own paragraph numbers and page numbers.
- Word-for-word checks of a quotation against a judgment, and against a named paragraph.
- Later Supreme Court judgments that cite a judgment, with the citing paragraph. These are
  citations, not treatment labels.
- The authorities a judgment cites, as printed in it.
- The table of old and new criminal code sections: IPC to BNS, CrPC to BNSS and the Indian
  Evidence Act to the BSA.
- No High Court or tribunal judgments yet.

All nine tools only read. None of them can change anything in your Vakilat account.

| Tool | What it does |
| --- | --- |
| `search_judgments` | Searches the judgments for a point of law, a provision, a judge or the parties |
| `find_by_citation` | Finds the judgment an SCC, AIR, SCR, SCC OnLine or INSC citation points to |
| `find_by_case_number` | Finds the judgment for a case number |
| `read_paragraphs` | Reads paragraphs by the Court's own numbers, word for word |
| `search_within` | Finds the paragraphs inside one judgment that discuss a point |
| `cited_by` | Lists later judgments that cite a judgment |
| `authorities_cited` | Lists the authorities a judgment cites |
| `check_citation` | Checks a citation, and whether a quotation is word for word in it |
| `old_and_new_code` | Maps an IPC, CrPC or Evidence Act section to the BNS, BNSS or BSA, and back |

## Connect

1. Add Vakilat to your assistant: install this plugin, or add `https://api.vakilat.io/mcp` as
   a connector. Step-by-step instructions for Claude, ChatGPT and Microsoft Copilot are on
   [app.vakilat.io/connect](https://app.vakilat.io/connect) once you are signed in. In Claude
   Code, install the plugin with:

   ```
   /plugin install vakilat --marketplace Vakilat/mcp
   ```

2. The assistant opens Vakilat's sign-in page. Sign in with the account you use on
   [app.vakilat.io](https://app.vakilat.io). Without a Vakilat account the add-on offers no
   tools, so create one there first.
3. Ask a question about Indian law, for example "Which judgment is (2014) 8 SCC 273?" or "What
   replaced section 438 CrPC?".

## Daily limit

Each Vakilat account has a daily number of tool calls per seat. Your limit and your use today
are shown on app.vakilat.io/connect. When the
limit is reached, the tool says so and says when it resets, at midnight India time.

## Data

Your conversation stays with the assistant you use, under your own account with it. Vakilat
receives only what each tool needs, such as a search query, a citation or a quotation, together
with your Vakilat sign-in. The tools never open your Vakilat matters, documents or Library.
Vakilat records each tool call with the tool's name, your account, the outcome and the time,
not the tool's arguments. The plugin files themselves send nothing; only the MCP server above
is contacted. See the [privacy notice](https://www.vakilat.io/privacy) and the
[terms](https://www.vakilat.io/terms).

## Limits

Vakilat is research help for lawyers, not legal advice. Check every authority before relying
on it; a qualified lawyer reviews any output before it is used for advice, a filing or any
decision.

## Support

Write to hello@vakilat.io, or see [vakilat.io/contact](https://www.vakilat.io/contact). Report
a security issue privately to security@vakilat.io.

## License

The files in this repository are under the MIT License. See [LICENSE](LICENSE). The Vakilat
service and its data are covered by the [terms](https://www.vakilat.io/terms).
