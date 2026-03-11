# Session History

## 2026-03-11 - Added Teebot and TallyDay projects

### What was done
- Added Teebot (teebot.dev) as the first project card with a Playwright screenshot thumbnail
- Added TallyDay (tallyday.onrender.com) as the last project card with a live screenshot showing a game in progress
- Added CSS support for screenshot-style thumbnails (`object-fit: cover`, full-width) vs icon thumbnails (96x96 rounded)
- Deployed all files to GreenGeeks via SCP

### Key details
- Hosting: GreenGeeks at `/home/hostfke5/public_html/software.foxpress.io/`
- SSH: `hostfke5@mtlr201.websitehostserver.net` with key `~/.ssh/greengeeks_foxpress`
- Deploy method: `scp` individual files to GreenGeeks (no build step, static HTML)
- Playwright installed for screenshots (`npx playwright screenshot`)
- TallyDay on Render has cold start delay; use `--wait-for-timeout=3000` for screenshots

### Files modified
- `index.html` - Added Teebot and TallyDay entries, screenshot CSS class
- `teebot-thumb.png` - Screenshot of teebot.dev (new)
- `tallyday-thumb.png` - Screenshot of tallyday.onrender.com mid-game (new)

### Current state
- 3 projects listed: Teebot, Subfolder, TallyDay
- Committed and pushed to GitHub (only the Teebot commit; TallyDay changes not yet committed)
- Deployed to GreenGeeks and live at software.foxpress.io

### Next steps
- Commit TallyDay addition to git
- Could add more projects as needed
