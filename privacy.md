# Markdown Fixer for Jira: Privacy Policy

_Last updated: 16 November 2026_

Markdown Fixer ("the app") is published by Ashraf Builds ("we"). This policy explains what the app does with data in your Jira site.

## The short version

- The app runs entirely on Atlassian's own infrastructure. It is a Forge app that is eligible for **Runs on Atlassian**.
- It sends **no data** to us or to any third party. It makes no outside network calls.
- It keeps only what it needs to work, and deletes undo copies after 7 days.

## What the app reads

It reads issue descriptions and comments in the projects an admin enables. It uses them to check for raw Markdown and to convert it into Jira formatting. It also checks whether an author is an app (bot) account.

## What the app stores, and for how long

All of this is kept in Atlassian-hosted Forge storage, inside your site's app installation.

| Data | Why | How long it is kept |
|---|---|---|
| Admin settings, which may include the account IDs of bot accounts an admin chooses | To know which projects and authors to fix | Until an admin changes them or the app is uninstalled |
| An undo copy of a description or comment, taken just before the app fixes it. It may contain @mentions. | So a user can undo the fix | **7 days**, then deleted automatically |
| A one-way hash of content a user chose to undo | So the app doesn't fix it again | 90 days |
| Forge app logs (issue key and the decision taken; no content) | Troubleshooting | According to Atlassian's Forge log retention |

## Personal data and your rights

The only personal data the app stores is Atlassian account IDs. They appear in the bot list and in @mentions inside undo copies. Every week the app reports these account IDs to Atlassian's Personal Data Reporting API, as Atlassian requires. When Atlassian reports that an account has been closed, the app deletes its data.

To have data deleted sooner, uninstall the app or contact us.

## Sharing

We do not sell, share or transfer your data. We do not see it.

## Contact

mohdashraf010897@gmail.com
