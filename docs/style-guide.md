# Style Guide

This guide ensures all pages in the project have a consistent look and feel.

## Theme

All pages use a **dark theme**. The color palette is defined in `assets/style.css` as CSS variables:

| Variable | Color | Usage |
|----------|-------|-------|
| `--bg-primary` | `#1e1e2e` | Page background |
| `--bg-secondary` | `#181825` | Header, sidebar |
| `--bg-surface` | `#252538` | Cards, panels |
| `--bg-hover` | `#313147` | Hover states |
| `--text-primary` | `#cdd6f4` | Main text |
| `--text-secondary` | `#a6adc8` | Secondary text |
| `--text-muted` | `#6c7086` | Muted/hint text |
| `--accent` | `#89b4fa` | Links, highlights |
| `--green` | `#a6e3a1` | Success, ready |
| `--yellow` | `#f9e2af` | Warning, coming soon |
| `--red` | `#f38ba8` | Error |
| `--orange` | `#fab387` | Badges, labels |
| `--border` | `#45475a` | Borders |

## HTML Template

Every new page should follow this basic structure:

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Page Title - Data Warehouse</title>
  <link rel="stylesheet" href="../assets/style.css">
  <!-- page-specific styles below, if needed -->
</head>
<body>
  <header class="site-header">
    <h1><span>Data</span> Warehouse</h1>
    <p class="subtitle">Page Description</p>
  </header>

  <!-- page content here -->

  <footer class="site-footer">
    <p><a href="../index.html">&larr; Back to Home</a></p>
  </footer>
</body>
</html>
```

## Rules

1. **Always reference `../assets/style.css`** — do not copy style definitions into individual pages.
2. **Use CSS variables** for colors — never hardcode hex values in page-specific styles.
3. **Font stack**: `'Segoe UI', 'PingFang SC', 'Microsoft YaHei', sans-serif` (inherited from the shared CSS).
4. **Code font**: `'Consolas', 'Fira Code', monospace`.
5. **Keep page-specific CSS minimal** — if a style is reusable, add it to `assets/style.css`.
6. **Content language**: Chinese. **File/directory names**: English.
