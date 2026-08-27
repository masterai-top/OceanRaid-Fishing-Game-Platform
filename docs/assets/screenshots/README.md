# Screenshot Publishing Checklist

Add authentic product screenshots with these exact names:

- `lobby.webp`
- `classic-mode.webp`
- `tournament-mode.webp`
- `sea-demon.webp`
- `jade-arena.webp`
- `admin-console.webp`

Recommended size: 1600 x 900 pixels, WebP, below 500 KB per image. Use clear gameplay images without artificial blur or heavy text overlays.

Before publishing, remove player names, account IDs, phone numbers, IP addresses, orders, payment records, access tokens, admin usernames, internal domains, QR codes, and debug information.

After adding the files, insert the following Markdown into the screenshot section of the root README:

```markdown
| Game lobby | Classic fishing | Tournament mode |
| --- | --- | --- |
| ![Arcade fishing game lobby](docs/assets/screenshots/lobby.webp) | ![Classic fish shooting gameplay](docs/assets/screenshots/classic-mode.webp) | ![Fishing tournament mode](docs/assets/screenshots/tournament-mode.webp) |

| Sea Demon Assault | Jade Arena | Operations console |
| --- | --- | --- |
| ![Sea Demon Assault mode](docs/assets/screenshots/sea-demon.webp) | ![Jade Arena fishing mode](docs/assets/screenshots/jade-arena.webp) | ![Node.js operations console](docs/assets/screenshots/admin-console.webp) |
```
