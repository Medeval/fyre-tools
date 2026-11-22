<p align="center">
  <a href="https://fyretools.net"><img src="./public/wordmark.png" alt="Fyre Tools" width="640"></a>
</p>

**Fyre Tools — the Ultimate Fyre Version.** A Guardian-branded fork of [Killer Tools](https://killertools.net), re-forged for adding my own tools alongside the original set.

Field techs don't have time for bloat. Every tool here exists because someone needed it on the job and couldn't find something that just worked without an account, an install, or telemetry.

This started as [Steve the Killer](https://theKiller.net)'s Killer Tools, which itself began as a fork of the excellent [IT-Tools](https://github.com/CorentinTh/it-tools) project by [Corentin Thomasset](https://github.com/CorentinTh). The upstream set covers looking up Group Policy settings mid-ticket, scanning a client's subnet, and pulling port references without leaving the browser — the [Killer Scripts](https://github.com/SteveTheKiller/killer-scripts) library covers everything that comes up every ticket cycle, running in PS 5.1, PS 7, and Kaseya LiveConnect with no dependencies.

Everything runs in your browser. Nothing is tracked. No account is required, ever.

Fyre Tools fork maintained by Medeval Fyre. Upstream Killer Tools built and maintained by [Steve the Killer](https://theKiller.net).

Use Killer Tools from an AI agent with [KillerTools MCP](https://killertools.net/mcp) (upstream).

---

## Notable Tools

A sampling of what's built into the site beyond the standard IT-Tools toolkit.

| Tool | Description |
|------|-------------|
| **Exchange NDR Lookup** | Look up Exchange and M365 bounce codes with plain-language cause and fix guidance |
| **Group Policy Reference** | Search common Windows GPO settings by name, path, registry key, or description |
| **Windows Error Code Lookup** | Hex or decimal lookup covering system errors, BSODs, WMI, RPC, and MSI errors |
| **Windows Event Lookup** | Event IDs with descriptions, severity levels, and common causes |
| **Domain Lookup** | WHOIS registration details and email DNS checks (MX, SPF, DKIM, DMARC) for any domain in a single view |
| **Email Header Parser** | Paste raw headers to trace the delivery hop chain and view auth results |
| **CVE Lookup** | Live search against the NIST NVD by ID or keyword |
| **Port & Protocol Reference** | Common ports and protocols with security notes and dangerous port flags |
| **M365 License SKU Decoder** | Convert Microsoft 365 license SKU strings and GUIDs to readable product names |
| **PowerShell Builder** | Pick a cmdlet, fill in parameters, and copy the finished command |
| **Killer Scripts** | PowerShell scripts for Windows administration and MSP field work |

---

## Killer Apps

Standalone executables for field work. No installer, no runtime, no dependencies.

| App | Description |
|-----|-------------|
| [KillerScan](https://KillerScan.net) | Fast network scanner. ARP and ping discovery, port probing, vendor lookup, and automatic device classification. |
| [KillerPDF](https://KillerPDF.net) | Portable PDF editor. View, annotate, OCR, merge, split, flatten, sign, and open password-protected files. |
| [KillerShell](https://KillerShell.net) | Free shell for power users. A file browser, a terminal and a text editor in one window, one tab strip and one set of keys. |
| [KillerNotes](https://KillerNotes.net) | Encrypted notepad for techs. Rich notes with inline images and tables, instant full-text search, tags and nested groups, and optional password protection for the whole database. |
| [The Killendar](https://Killendar.net) | Encrypted desktop calendar. Month, week, day and agenda views, colour categories, iCalendar import and export, and appointments that stay in one file on your own machine. |

---

## Development

### Requirements

- [Node.js](https://nodejs.org/) 18+
- [pnpm](https://pnpm.io/)

### Setup

```sh
pnpm install
```

### Dev server

```sh
pnpm dev
```

### Build for production

```sh
pnpm build
```

### Tests

```sh
pnpm test
```

### Lint

```sh
pnpm lint
```

### Create a new tool

```sh
pnpm run script:create:tool my-tool-name
```

This generates the boilerplate in `src/tools/` and adds the import to `src/tools/index.ts`. Add the tool to the appropriate category and build it out from there.

### Recommended VS Code extensions

- [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (disable Vetur)
- [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin)
- [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)

Recommended workspace settings:

```json
{
  "editor.formatOnSave": false,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  }
}
```

---

## Contributing

Open a feature request or bug report in the [issues section](https://github.com/SteveTheKiller/killer-tools-site/issues/new/choose). I read them.

If this saves you time on the job, [buying me a coffee](https://www.buymeacoffee.com/StevetheKiller) is appreciated but never expected.

---

## License

This project is under the [GNU GPLv3](LICENSE).
