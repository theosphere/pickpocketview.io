# pickpocketview.io

A small, hand-crafted project gallery. One page, no build step, no
framework — just `index.html`.

Live at [pickpocketview.io](https://pickpocketview.io) once DNS is pointed
at GitHub Pages (see below); until then, at
https://theosphere.github.io/pickpocketview.io/.

## Adding a project

Copy the `<a class="card">` block in `index.html` and fill in the link,
title, and description. Swap the placeholder SVG inside `.card-image` for
a real screenshot (`<img>` instead of the inline SVG) once one exists.

## Custom domain setup (not yet done)

A `CNAME` file pointing at `pickpocketview.io` is already committed. To
actually serve there, add these DNS records at the domain's registrar:

- Four `A` records for the apex (`pickpocketview.io`) pointing at GitHub
  Pages' IPs: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`,
  `185.199.111.153`
- (Optional) a `CNAME` record for `www` pointing at
  `theosphere.github.io`

Then enable "Enforce HTTPS" for the custom domain in the repo's Pages
settings once DNS has propagated.
