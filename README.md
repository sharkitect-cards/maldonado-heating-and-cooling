# Maldonado Heating & Cooling — Digital Business Card

**Live card:** https://cards.sharkitectdigital.com/maldonado-heating-and-cooling/
**NFC / QR target:** https://cards.sharkitectdigital.com/maldonado-heating-and-cooling/contact.vcf

Program the physical NFC card and the printed QR with the **`contact.vcf` URL**, not the card page.
GitHub Pages serves `.vcf` as `text/x-vcard`, so a tap or scan opens "Add Contact" directly with the
logo attached — no extra taps.

## Contact on the card

| Field | Value |
|---|---|
| Name | Carlos Maldonado |
| Company | Maldonado Heating & Cooling |
| Phone | (913) 963-5392 |
| Email | maldonadolarios1987@gmail.com |
| Facebook | https://facebook.com/juancarlos.maldonadolarios |
| Tagline | Two Seasons. One Standard. |
| Services | Heating, Cooling, Installation & Repair |
| Area | Kansas City Metro |

## Intentionally omitted (not fabricated)

Website, office address, booking link, and job title. No data existed for these at build time.
They strip cleanly the same way the `_template` optional blocks do. **Backfill them in place**
(edit `index.html` + `contact.vcf`) when Carlos has them — this is a normal update, not a rebuild.

## Files

| File | Purpose |
|---|---|
| `index.html` | The card page. Split orange→blue accents sampled from the logo. |
| `contact.vcf` | vCard 3.0 with the logo embedded as `PHOTO`. **The NFC/QR target.** |
| `qr-code.svg` | On-page QR modal image (points at `contact.vcf`). |
| `logo.jpg` | Card logo, 800×800. |
| `manifest.json` | PWA manifest for "Add to Home Screen". |

## Brand

Sampled from the client logo: flame `#DD3002`, ice `#005BC3`. Lifted to `#FF6A28` / `#3B9EFF`
for legible contrast on the `#1A1A1A` card body.

---
Built by [Sharkitect Digital](https://www.sharkitectdigital.com) · 07/27/2026
