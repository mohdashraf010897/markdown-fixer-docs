# Markdown Fixer for Jira: Documentation

Markdown Fixer turns raw Markdown into proper Jira formatting. Jira shows Markdown as plain text when it is posted by bots, AI agents and integrations: things like `## headings`, `**bold**`, bullets, tables and code fences. Markdown Fixer converts that text into headings, lists, tables and code blocks.

## Setup (2 minutes, Jira admin)

1. Install the app from the Atlassian Marketplace.
2. Go to **Jira settings → Apps → Markdown Fixer**.
3. Switch **Automatic fixing** on.
4. Optionally, limit it to some projects (for example `ENG, OPS`).
5. Choose whose content to fix:
   - **App accounts** (on by default) covers integrations such as GitHub, Slack and AI agents.
   - **Account IDs**: list bots that post as a normal user account.
   - **Everyone**: fixes all authors. This is not recommended.
6. Click **Save settings**.

Automatic fixing is **off** until an admin switches it on.

## What gets fixed

| Bots post... | ...and readers see |
|---|---|
| `## Summary` | A heading |
| `**bold**`, `_italic_`, `~~strike~~`, `` `code` `` | The same formatting |
| `- item`, `1. item`, `- [ ] task` | Bullets, numbered lists, task lists |
| Fenced code with a language | A code block with syntax highlighting |
| GFM tables | A Jira table |
| `> quote`, `<details>` | A quote, an expand section |
| `[text](https://…)` | A link |

Fixes usually appear within **15–30 seconds**. Jira can take up to 3 minutes to send the app the event.

## When the app does nothing (by design)

- The text is already formatted, or is written in Jira wiki markup (`h2.`, `{code}`, `# numbered`).
- The text doesn't clearly look like Markdown.
- Converting would lose any word of the original. Then it skips the fix rather than risk losing content.
- The author isn't enabled in settings.

## Edit as Markdown

On any issue, open **••• → Edit as Markdown** to edit the description as Markdown, preview it, and save it back as Jira formatting. You can also copy the Markdown from there.

Mentions, panels and attachments show as ⟦tokens⟧. Leave them in place to keep them.

## Undo

If an automatic fix isn't what you wanted, open **••• → Edit as Markdown** and click **Undo automatic fix**. This is available for 7 days.

The app won't fix that content again unless the bot posts something new. Undo is refused if someone has edited the text since the fix, so that edit is never lost.

## Privacy

Nothing leaves Atlassian. See the [privacy policy](privacy).

## Support

mohdashraf010897@gmail.com. Please include the issue key and roughly when it happened.
