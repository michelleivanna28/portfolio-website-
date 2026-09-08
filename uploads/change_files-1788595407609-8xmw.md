# Homepage — build spec

Portfolio site for Michelle Ivanna, designer. Currently in Taipei, targeting brand / product / UI-UX roles.

Concept: a record catalogue. Existing visual language to preserve: subtle light-leak treatment, very subtle fluid background animation, words as the primary visual element.

**Scope note: only the sections below change. Everything not mentioned here stays exactly as it is.**

---

## 1. Header

Left: `Michelle Ivanna` — links to homepage.

Right: `ABOUT` · `CV` · `CONTACT`

- Collapses to a hamburger menu on mobile.
- **Blog is removed.** There is no blog content yet. It is replaced by CV, which links to a downloadable PDF or a dedicated page.

---

## 2. Hero — UNCHANGED

Keep the existing hero exactly as built: large display type, filled-on-scroll effect, italic words that pop up an image on hover.

```
Hi! I'm Michelle
a Designer working across
UI/UX, Brand, and Product
```

Images behind the italic words are already decided. Do not change the wording, the italics, or the scroll-fill behaviour.

---

## 3. Subtext — REPLACE

Replace the current subtext entirely. New copy:

```
Previously: multimedia marketing at a B2B SaaS company.
Now looking for the next problem to obsess over.
```

Then a third, quieter meta line below it:

```
Taipei, 4:12 PM — open to brand, product, and UI/UX
```

- The time is **live** and updates. Asia/Taipei timezone, rendered in local format.

---

## 4. Work section

Section heading: `Work Archive`

### Filter — NEW

Three options, sitting on the same baseline as the `Work Archive` heading, aligned right:

```
Work Archive                              All   Brand   Product
```

- Plain text, no pills, no boxes, no segmented-control chrome. Generous spacing between the three.
- Active option is at full opacity; the other two sit around 40%. That's the entire state indicator.
- On mobile the row drops below the heading, left-aligned, same treatment.
- Default state is **All** — all six projects in the existing 3×2 grid.
- `Brand` and `Product` each show 3, which reflows to a clean single row.
- Reflow is a short quiet transition. No staggered card entrances, no fade-up on each card.
- No counts next to the labels.

### Project assignment

| Project | Filter |
|---|---|
| Starise | Brand |
| Orion Suite | Brand |
| Beyond Being | Brand |
| AI Feature | Product |
| iManager Onboarding | Product |
| Taipei People | Product |

### Cards — UNCHANGED

Card layout, discipline labels, and styling all stay as they are.

### Removed

The existing **remastered / demo track** toggle comes off the homepage. Two toggles competing over six projects is noise. That idea moves to the individual case study pages later, where it controls depth — not on this page.

---

## 5. Closing section — NEW

After the work grid, one short section whose only job is to send people to the about page.

- A simple horizontal line as a shelf, with three or four book spines standing on it, seen edge-on with vertical titles.
- One line of copy above it:

```
Six projects, and about eleven other interests.
```

- Clicking the shelf or any spine goes to `/about`.
- This is a teaser, not the real shelf — spines don't need to be pullable here.

---

## 6. Global

- Motion stays subtle. The scroll-fill hero and the italic hover images are the two expressive moments; nothing new competes with them.
- Respect `prefers-reduced-motion` — when a visitor has that setting on, disable the background animation and the scroll-fill.
- Visible keyboard focus on the nav links, the three filter options, and the project cards. This means: when someone tabs through the page with a keyboard instead of clicking, whatever is currently selected needs a visible outline so they can see where they are. Style it to match the site — a thin ring or an opacity shift is fine — just don't remove it.
- Fully responsive down to mobile.
