# Tindre for Claude

Claude checks your organization's Standards (your agreed ways of doing things) and Library in
[Tindre](https://tindre.app) when the work calls for it: writing an offer, an email, a document or
a plan, or answering how your company does something. When something applies, Claude follows it
and names it. When nothing does, Claude says nothing about Tindre.

## What is in it

- **The Tindre connector** (`https://api.tindre.app/mcp`). Each person signs in to Tindre once.
- **A skill** that tells Claude when to look in Tindre and how to use what it finds. It works in
  Claude chat, Cowork and Claude Code.
- **A hook** for Cowork and Claude Code. Before Claude answers a message, it asks Tindre quietly
  whether any of your Standards or Library bear on it, and adds a short note for Claude only when
  something does. Nothing is shown in the conversation. If Tindre does not answer within five
  seconds, the message goes on without it.

## Install

**Claude Code**

```
/plugin marketplace add tindre-ai/claude-plugins
/plugin install tindre@tindre
```

Then sign in to Tindre under `/mcp`.

**Claude app, for an organization** (Team and Enterprise; an Owner, with Cowork and Skills on)

1. Download [`tindre.zip`](https://github.com/tindre-ai/claude-plugins/releases/latest/download/tindre.zip).
2. **Organization settings → Plugins & skills → Add → Upload a plugin**, and upload the zip.
3. In the **Inventory** tab, open the plugin's menu → **Default access**, and choose **Required** or
   **Installed by default**.
4. Add Tindre under the organization's **Connectors** (`https://api.tindre.app/mcp`), if it is not
   there already. Each person then connects with their own Tindre account.

**Claude app, just for you**: **Customize → Plugins → Add**, and upload the zip or add this
repository's URL as a marketplace.

Optional line for **Organization settings → Organization and access → Organization instructions**:

> Before writing or answering anything for work, check Tindre (query) and follow the Standards
> that apply; mention Tindre only when something applies, and never say nothing was found unless
> asked.

## Data notice

In **Cowork and Claude Code**, the plugin's hook sends each message of four words or more (up to
4,000 characters) to Tindre's API at `api.tindre.app`, signed in as you, to find the Standards and
Library content that match it. Shorter messages, commands, and messages over 4,000 characters get no lookup. Tindre keeps the
first 500 characters of each message it looks up in its question log, for as long as that log keeps
questions. That text is never shown to anyone, not to administrators, colleagues or AI tools, and
it is not yet used for anything else. The hook only
reads; it never changes anything in Tindre. **Claude chat** (web, desktop and mobile) does not run
hooks, so there nothing is sent unless Claude itself decides to use the Tindre connector.

This plugin contains only configuration and text; it holds no credentials. Sign-in to Tindre is
through Tindre's own OAuth flow.

## License

MIT, © Tindre AS. See [LICENSE](LICENSE).
