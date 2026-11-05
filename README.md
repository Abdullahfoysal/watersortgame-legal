Template for the public legal site (privacy policy, terms, landing page). Placeholders: APP_NAME, DEVELOPER_NAME, CONTACT_EMAIL, DATE, GOVERNING_LAW_COUNTRY, ANALYTICS_RETENTION.
Published copy lives in `site/` (its own git repo → github.com/Abdullahfoysal/waterpouring-legal, GitHub Pages from main / root; ignored by the game repo).
To regenerate after editing the template:
1. `rsync -a --delete --exclude .git --exclude README.md docs/compliance/site-template/ site/`
2. `tools/fill_site_placeholders.sh --dir site --app-name "Glassly: Water Sort Puzzle" --developer "Gayen BD" --email gayenbd@gmail.com --date "<D Month YYYY>" --law Bangladesh --retention "2 months"`
3. Commit + push inside `site/`. Re-date and update when ads or purchases ship.
