### On GitHub, when you view a .md (Markdown) file in the repository,
👉 only images (and plain links, text, code, tables, etc.) are actually rendered inline.

## Everything else — like .doc, .pdf, .mp4, .html, .iframe, .embed, etc. — is blocked or escaped for security reasons.

---

### 💡 GitHub Markdown Rendering Rules

Here’s the simple truth:
File / Tag	Inline Preview	Why
<pre>
  🖼️ Images (.png, .jpg, .gif, .svg)	✅ Works	Safe & supported by Markdown spec
  📄 .doc / .docx	❌ No	Treated as downloadable binary
  📘 .pdf	❌ No	Must click to open; not embedded
  🎥 Videos / Audio	❌ No	HTML tags stripped
  🧩 <iframe> / <embed> / <object>	❌ No	Security sandbox blocks them
  🔗 Links ([text](url))	✅ Works	Markdown-safe and sanitized
  ✅ What You Can Do on GitHub
</pre>
---
Here’s what’s possible and safe inside .md on GitHub:

#### ✅ Works fine

![Logo](https://github.com/hsj71/Flask/raw/main/logo.png)

[Download Word file](https://raw.githubusercontent.com/hsj71/Flask/main/f.doc)

[Read project documentation](https://hsj71.github.io/Flask/)

That’s all GitHub supports inline — images and links.

---

🚀 If You Want Inline Previews for Other Files

Then you need to move beyond GitHub’s Markdown sandbox:

Use GitHub Pages (convert your .md → .html).

Or use VS Code / Obsidian / Typora locally (they render iframes properly).

Or convert .doc → .pdf or .png and embed as image.

---

🧭 TL;DR

✔️ GitHub Markdown supports inline images
✔️ Supports clickable links to any file
❌ Does not support inline .doc, .pdf, or <iframe>

---
