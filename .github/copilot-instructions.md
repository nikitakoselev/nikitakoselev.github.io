# Copilot repository instructions (nikitakoselev.github.io)

This repository is a public GitHub Pages Jekyll site. It is the canonical “home base” for:
- Recognitions (external validation)
- Artefacts (writing, talks, open-source links)
- A legacy archive of older blog posts/pages

Branch rule
- Work only on the existing branch: chore/site-recognitions-openuk-2026.
- Do NOT create new branches.

Safety / “do not create a mess”
- Do not delete existing content. Prefer archiving by moving to /archive and preserving access via links.
- Do not modify Jekyll/theme internals unless necessary to fix a build issue:
  _config.yml, Gemfile/Gemfile.lock, _layouts/, _includes/, theme CSS/JS, and any GitHub Actions workflow files.
- Avoid changing existing URLs. If you must move a page that had an existing URL, preserve it using either:
  - a stub page at the old path that links to the new location, or
  - Jekyll front matter `permalink:` to keep the original URL.

Content and writing rules
- Keep all public writing free of employer/internal-work details.
- Use a calm, practical tone; avoid hype/marketing language.
- Use clear headings, short paragraphs, and bullet lists where helpful.

Structure conventions
- Prefer folders with `index.md` for sections (e.g., /recognitions/openuk-honours-2026/index.md).
- Add YAML front matter to new Markdown pages for consistency (at minimum `title:`; include `layout:` only if the repo already uses it).
- Prefer relative links within the site.

Git hygiene
- Keep commits small and reviewable.
- Update `.gitignore` safely (macOS, IDE files, common build outputs).
- Remove tracked junk files only if they are actually tracked in the repo.
