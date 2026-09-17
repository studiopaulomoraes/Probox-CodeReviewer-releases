# Screenshots

PNG files in this folder are embedded in the root `README.md` and published on GitHub Pages.

## Files

| File | Screen | Content shown |
|------|--------|---------------|
| `01-pr-input.png` | PR input | Marketing demo tabs for GitHub, GitLab, Bitbucket, and Azure DevOps with the PR URL field and Start button |
| `02-overview.png` | Overview | GitLab demo PR with description markdown and chronological remote thread feed |
| `03-commits.png` | Commits | Bitbucket demo PR with commit list (message, author, SHA, date) and multi-select toolbar |
| `04-diff-files.png` | Diff files | Bitbucket demo PR with file list, side-by-side diff, and AI review panel |
| `05-comments.png` | Comments | GitHub demo PR with inline AI findings in the diff and draft comments ready to post |
| `06-ai-review.png` | AI review | AI Review dialog (model, effort, technology, context, language) over a loaded diff |
| `07-settings.png` | Settings | Appearance, language, sound, PR updates, security PIN, and Manage PATs |
| `08-about.png` | About | Version, credits, and Probox Studio links |

## Capture workflow

From the Code Reviewer repository:

```bash
./scripts/marketing/capture-desktop-screenshots.sh
```

This generates PNGs under `marketing-screenshots/<timestamp>/` and copies them here when `../Probox-CodeReviewer-releases` exists (override with `CODE_REVIEWER_RELEASES_DIR`).

To sync an existing folder manually:

```bash
./scripts/marketing/sync-screenshots-to-releases.sh marketing-screenshots/<timestamp>
```

## Tips

- **Resolution:** 1440×900 or 1920×1080 works well on GitHub Pages.
- **Format:** PNG preferred for UI captures.
- **Privacy:** Demo fixtures use fictional repo names; still avoid real tokens or emails before committing.

After updating images, commit and push to `main` — GitHub Pages updates automatically.
