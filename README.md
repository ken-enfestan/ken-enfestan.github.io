# Your portfolio site

A single-file HTML/CSS/JS portfolio template — editorial layout, big serif
headlines (Fraunces) paired with a clean grotesk sans (Archivo), a numbered
work index, and a floating image preview that follows the cursor when you
hover a project on desktop.

## Customize it

Everything lives in `index.html`. Open it in any text editor and update:

1. **Your name & tagline** — top of `<aside class="sidebar">` and the `<h1>`
   in the hero section.
2. **Projects** — each project is a `<li>` inside `<ul class="work-list">`.
   Duplicate a block to add more, or delete ones you don't need. Update:
   - `data-preview="..."` — swap in the path to your own image
     (e.g. `images/kite-ember.jpg`)
   - the title, medium, and year text
   - `href="#"` — point it at a case study page if you build one, or an
     external link
3. **About section** — swap in your bio and the `capabilities` list.
4. **Contact** — update the email address (appears twice: sidebar footer
   and the contact section) and social links.
5. **Colors** — at the top of the `<style>` block, the `:root` section has
   named variables (`--paper`, `--ink`, `--accent`, `--moss`). Change the
   hex values to shift the whole palette.

## Add your images

Create an `images` folder next to `index.html`, drop your project images in,
and point each project's `data-preview` at the right file, e.g.:

```html
data-preview="images/kite-ember.jpg"
```

Keep images reasonably sized (under ~500KB each) so the site loads fast —
tools like TinyPNG or Squoosh work well for this.

## Put it on GitHub Pages

1. Create a new repository on GitHub named `yourusername.github.io`
   (replace `yourusername` with your actual GitHub username).
2. Upload `index.html`, this `README.md`, and your `images` folder into
   that repo (drag-and-drop on github.com works, or use git/GitHub Desktop).
3. Go to the repo's **Settings > Pages** and confirm the source branch is
   set to `main`.
4. Your site will be live at `https://yourusername.github.io` within a
   few minutes.

Want a custom domain instead of the `.github.io` address? GitHub's docs
under **Settings > Pages > Custom domain** walk through pointing a
purchased domain at your Pages site.
