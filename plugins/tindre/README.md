# Tindre

The operating system for AI in your organization, in Claude.

With this plugin, Claude checks your organization's Standards and Knowledge in
[Tindre](https://www.tindre.ai/en) when the work calls for it, such as writing an offer, an email or
a document, or answering how your company does something. When a Standard applies, Claude follows it
and names it in one short line, linked to Tindre; when nothing applies, Claude says nothing about
Tindre. It works in Claude chat, Cowork and Claude Code. Your organization needs a Tindre account.

## Install

**Claude Code**

```
/plugin marketplace add tindre-ai/claude-plugins
/plugin install tindre@tindre
```

**Claude app, for an organization** (Team and Enterprise; an Owner, with Cowork and Skills on)

1. Download [`tindre.zip`](https://github.com/tindre-ai/claude-plugins/releases/latest/download/tindre.zip).
2. **Organization settings → Plugins & skills → Add → Upload a plugin**, and upload the zip.
3. In the **Inventory** tab, open the plugin's menu → **Default access**, and choose **Required** or
   **Installed by default**.
4. Add Tindre under the organization's **Connectors** (`https://api.tindre.app/mcp`), if it is not
   there already.

**Claude app, just for you**: **Customize → Plugins → Add**, and upload the zip or add this
repository's URL as a marketplace.

## Sign in

Each person signs in to Tindre once, with their own Tindre account, through Tindre's own sign-in. In
Claude Code, sign in to the plugin's Tindre server under `/mcp`; in the Claude app, connect Tindre
from the Connectors tab. Claude sees only what that person may read in Tindre.

## Links

[Privacy](https://tindre.ai/legal/privacy) · [Terms](https://tindre.ai/legal/terms) ·
[Support](https://www.tindre.ai/support)

## License

MIT, © Tindre AS. See [LICENSE](LICENSE).
