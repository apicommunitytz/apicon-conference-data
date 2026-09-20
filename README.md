# APICon conference data

Public JSON for the APICon companion app. The app can update schedule, speakers, and About content by changing this file — without an App Store or Google Play release.

```text
apicon-conference-data/
└── 2026/
    └── conference.json
```

The document matches the app’s `Conference` type. Organizer photos stay bundled in the app; they are not in this JSON.

## Repository page vs raw file

| URL | What it is |
| --- | --- |
| `https://github.com/apicommunitytz/apicon-conference-data` | GitHub **website** (HTML). The app cannot parse this as conference data. |
| `https://raw.githubusercontent.com/apicommunitytz/apicon-conference-data/refs/heads/main/2026/conference.json` | **Raw file**. Plain JSON over HTTPS. This is what `fetch` will request. |

The shorter `/main/` form of a raw URL usually works too. Both mean “the file on the `main` branch.”

## Publish

This folder is a local git repo. Create `apicommunitytz/apicon-conference-data` on GitHub, then:

```bash
git remote add origin https://github.com/apicommunitytz/apicon-conference-data.git
git push -u origin main
```
