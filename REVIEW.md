# Review notes

This repo is Joe's GitHub profile README. One file, no code, no dependencies, no build — whatever is in `README.md` renders publicly at <https://github.com/joe-bell>. Review is about what the page says and whether it still renders.

- **The whole README is a single linked image** — `[<img ...>](...)`. If that image URL stops resolving, the profile page is blank. On any PR that touches it, check the `github.com/joe-bell/joe-bell/assets/...` URL still returns 200.
- **The `alt` text is the only text on the page.** It transcribes the tweet in the image, so screen readers and link previews depend entirely on it. If the image changes, the alt text must change with it.
- **The link points at `twitter.com`**, which currently 301-redirects to `x.com`. Fine today — flag it if it ever breaks, since it's the README's only link.
- **Everything here is public.** Flag anything added that Joe may not want on his public profile: email addresses, employer or client detail, personal specifics.
- **Keep the raw `<img>` HTML.** GFM allows it, and it carries the `width` and `alt` attributes; plain markdown image syntax would drop both.
- **Host images on GitHub** (repo assets or user-attachments), not third-party hosts — those rot and can add tracking to a page Joe doesn't control the traffic of.
