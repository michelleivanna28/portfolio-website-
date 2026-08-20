# Michelle Ivanna — portfolio site

Static site. No build step, no dependencies. Any static host serves it as-is.

## Files

- `index.html` — the whole site (homepage + all six case studies)
- `support.js` — runtime the page needs; must stay next to `index.html`
- `uploads/` — every image the site loads

```
uploads/
  me.png
  thumbnails/       homepage project thumbnails
  starise/          + guidelines/, versions/
  ai-feature/
  orion/
  imanager/
  beyond-being/
  taipei-people/
```

One folder per project, all lowercase. Don't add a folder whose name differs from an existing one only by capitalisation — Mac and Windows treat those as the same folder and will merge them on upload, while the live server won't.

## Deploy (GitHub + Vercel)

1. Upload the contents of this folder to the repo root — `index.html` at the top level, not inside a subfolder.
2. Delete the old `uploads/Web`, `uploads/Website` and `uploads/my site thumbnail` folders from the repo; they are replaced by the structure above.
3. vercel.com → sign in with GitHub → **Add New → Project** → pick the repo.
4. Framework preset **Other**; leave build command and output directory empty. Deploy.

## Updating

Changes land on a branch first, so Vercel builds a preview URL before anything reaches the live site. Approve by merging the branch into `main`.

## Known gaps

- Taipei People's UI & animation clips are placeholders. Re-export as MP4/H.264 720p, roughly 1–2 MB each.
- iManager's visuals are marked coming soon in four places.
- `uploads/me.png` is 2.3 MB — worth compressing.
