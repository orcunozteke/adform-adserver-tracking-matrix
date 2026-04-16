# Adform — Ad Server Walled-Gardens Tracking Matrix

An interactive reference for agency trafficking teams: where Adform click and impression trackers are supported across walled-garden platforms, how to implement them, and where they aren't supported.

**🌐 Live site:** `https://<your-username>.github.io/<repo-name>/`

## What this covers

- **10 platforms** — Meta, Google Ads, DV360, TikTok, LinkedIn, Snapchat, Reddit, Pinterest, X, Microsoft Advertising
- **49 platform × ad-format combinations**
- For each: click support, impression support, UI path, API field, implementation example, known limitations, confidence grade
- Three views: click tracking only, impression tracking only, side-by-side

## How to use it

1. **Search** by platform, ad format, or setup term (e.g. "Meta DPA", "Performance Max", "LinkedIn lead gen")
2. **Filter** by platform or support status using the chips at the top
3. **Switch channels** between Click, Impression, or Side-by-side views
4. **Click any row** to expand the implementation details (UI path, API field, example snippet, limitations)
5. **Copy a link** to a specific row to share with colleagues — the URL captures the full view state including filters and the expanded row
6. **Export CSV** to pull a filtered shortlist into a trafficking brief or ticket

## Data quality — please read

**Click-tracker data** is sourced from official platform documentation and verified by Adform's tracking team.

**Impression-tracker cells marked `ASSUMED`** are inferred from published platform policy (allowlists, partner tiers, general 3P-tag behaviour) and are **pending direct verification**. Treat them as a best-informed starting point, not as a final implementation guarantee.

**Confidence grades:**

| Grade | Meaning |
|-------|---------|
| **A** | Verified against official platform docs |
| **B** | Likely based on partial evidence or policy analogy |
| **D** | Unverified — validate with your Adform AM before setup |

For high-spend or novel placements, always test before production launch and confirm with your Adform contact.

## Support status legend

- **Supported** — officially documented and production-ready
- **Conditional** — works with caveats (e.g. account-level only, specific campaign types, claimed-domain requirements)
- **Not supported** — platform does not permit Adform tracking in this surface
- **Unknown** — no primary platform statement found; verify with Adform AM

## Source data

- Last verified: **6 March 2026**
- Source platform documentation links are available on request from your Adform contact
- Data updates are committed to this repo and take effect within ~1 minute of push

## Contributing / corrections

Found something outdated or wrong? Open an issue in this repo or contact your Adform account team. When platforms update their tracking policies, please flag the affected rows so the source data can be re-verified.

## Local preview

Because it's a single self-contained HTML file with no dependencies, you can preview locally by just opening `index.html` in any modern browser — no build step required.

---

*Maintained by the Adform tracking team. For escalations or custom walled-garden implementation support, contact your Adform AM.*
