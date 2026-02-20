# Paste Clean

**Stop reformatting text every time you move it between apps.**

[pasteclean.coderkuttappan.com](https://pasteclean.coderkuttappan.com)

Paste Clean is a smart clipboard cleaner that understands where your text came from and where it's going. Pick the source app, pick the destination — get perfectly formatted text.

## How It Works

1. **Paste** your text into the input box
2. **Pick the source** — Paste Clean auto-detects it, or you can choose manually (Outlook, Gmail, Word, PDF, Excel, Markdown)
3. **Pick the destination** — Markdown, Outlook, Gmail, Word, or WhatsApp
4. **Copy** the cleaned output

Everything runs in your browser. Nothing is sent to any server.

## What It Fixes

- Outlook/Word formatting garbage (MSO styles, broken lists, `<o:p>` tags)
- Gmail wrapper cruft and signatures
- PDF line breaks and hyphenation artifacts
- Marketing email layout tables and tracking pixels
- Mojibake (UTF-8 decoded as Windows-1252)
- Zero-width characters, non-breaking spaces, extra whitespace

## Features

- **Auto-detect**: Paste anything and Paste Clean suggests the right source mode
- **Source-aware cleaning**: Each input mode has a specialized normalizer
- **Destination-aware formatting**: Output is styled for the target app (inline CSS for email clients, WhatsApp-native formatting, clean Markdown)
- **Font/size overrides**: Customize font family and size for Word, Outlook, and Gmail output
- **Dark mode**: Follows system preference with manual toggle
- **No backend**: Pure client-side HTML/CSS/JS, no build step

## Tech Stack

- Vanilla HTML/CSS/JS (single file)
- [Tailwind CSS](https://tailwindcss.com/) via CDN
- [marked.js](https://marked.js.org/) — Markdown to HTML
- [Turndown](https://github.com/mixmark-io/turndown) — HTML to Markdown
- [turndown-plugin-gfm](https://github.com/mixmark-io/turndown/tree/master/packages/turndown-plugin-gfm) — GFM table support

## License

MIT
