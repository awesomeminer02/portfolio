# CJ Petka — Engineering Portfolio

A single static page: `index.html` plus the `images/` folder. No build step, no dependencies.

## Put it online with GitHub Pages

1. On GitHub, create a new **public** repository named `portfolio`.
2. Upload `index.html`, `README.md`, and the whole `images/` folder
   (drag them into the repo page, or `git push` from your machine).
3. Go to **Settings → Pages**. Under "Build and deployment," set Source to
   **Deploy from a branch**, pick **main** and **/ (root)**, and click **Save**.
4. After a minute or two the site is live at
   `https://awesomeminer02.github.io/portfolio/`

## Add your own domain (e.g. cjpetka.com)

1. Buy the domain at a registrar (Cloudflare, Porkbun, Namecheap).
2. In the registrar's DNS settings, add the records from GitHub's guide,
   "Managing a custom domain for your GitHub Pages site":
   four **A** records for the bare domain pointing at GitHub's Pages IPs,
   and a **CNAME** record for `www` pointing at `awesomeminer02.github.io`.
   Copy the IPs from that guide rather than from anywhere else.
3. Back in **Settings → Pages**, type `cjpetka.com` under "Custom domain,"
   click **Save**, then tick **Enforce HTTPS** once it becomes available.
4. Recommended: verify the domain in your GitHub account settings
   (**Settings → Pages → Add a domain**) so no one else can claim it on GitHub.

DNS can take from a few minutes to a day to start working.

If you change your GitHub username later, a custom domain keeps working;
just update the `www` CNAME record to the new `username.github.io`.

## Editing

- **Text:** everything is plain HTML in `index.html`; each project is one `<section>`.
- **Swapping a photo:** replace the file in `images/` with one of the same name.
  If the new photo has a different shape, also update that image's
  `width`/`height` attributes and the `--r` value on its `<figure>`
  (width divided by height) so the row lines up again.
- **CAD screenshots:** `rail-cad.jpg` (about 1.38:1) and `car-cad.jpg` (2:1)
  are the two photos of a monitor worth replacing first.
