# Neonix MCP

> Neonix is an HTML-to-motion-video compiler: it turns HTML and CSS into a real, exportable motion video.

Neonix MCP is the official [Model Context Protocol](https://modelcontextprotocol.io) server for
Neonix. Connect Claude, ChatGPT, Grok, or any other MCP client to create, edit, preview, and
export motion-video projects directly from HTML and CSS — no separate API integration required.

## How it works

```text
HTML/CSS  →  JSON  →  Editor  →  Export video
```

Write HTML and CSS describing a scene — yourself, or have an AI agent write it — and Neonix
compiles it into a structured JSON document you can preview and edit, then exports it to a real
MP4.

## Connect

Remote endpoint: `https://www.neonix.video/api/mcp` (Streamable HTTP, OAuth 2.1 — sign in with
your Neonix account, no API key required).

**Claude Code**

```bash
claude mcp add --transport http neonix https://neonix.video/api/mcp
```

**Claude, ChatGPT, or any other MCP client** — add a remote server pointing at the endpoint
above and complete the OAuth sign-in when prompted.

## What you can do

- **Projects** — create, list, read, update, and delete Neonix video projects
- **HTML authoring** — read, edit, validate, and compile the HTML/CSS source of a project
- **JSON patches** — apply small, validated edits directly to the compiled document
- **Assets** — upload, import, and attach images, video, and audio to a project
- **Export** — render a project to a real MP4 and get a download link
- **Editor & preview** — open a project in the Neonix web editor or a live preview

## Links

- Website: https://www.neonix.video
- Docs: https://www.neonix.video/docs
- Overview: https://www.neonix.video/overview
- CLI scaffolder (`create-neonix`): https://github.com/neonix-video/html-to-video

## License

MIT — see [LICENSE](./LICENSE).
