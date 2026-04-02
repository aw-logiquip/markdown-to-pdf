# Markdown to PDF - Status Updates

**Last Updated:** 2026-04-02

---

## Session: 2026-04-02

### Session Summary
Added open-in-new-tab behavior for PDF and HTML exports. The main export button now opens the rendered output in a new browser tab instead of forcing a download. A dedicated download button was added for users who want to save files locally.

### Session Metrics
- **Productivity**: Very productive
- **Energy/Mood**: Energized
- **Blockers**: None
- **Issues**: None

### Activities Completed
- [x] Modified export behavior to open PDF/HTML/Markdown in new browser tab by default
- [x] Added dedicated download button (down arrow) to the export button group
- [x] Updated `exportPDF()` to use `pdf.output('blob')` + `window.open()` for open mode
- [x] Updated `exportHTML()` and `exportMD()` to support both open and download modes
- [x] Added `openInTab()` helper function for blob URL new-tab opening
- [x] Added `runDownload()` function to route download actions
- [x] Updated button labels and format switching logic
- [x] Committed and pushed to GitHub

### Files Modified
- `index.html` — 43 insertions, 12 deletions (export logic + UI button changes)

### Next Steps
- Test export-in-new-tab across different browsers (Chrome, Edge, Firefox)
- Consider adding a user preference to remember open vs download preference
- Evaluate if Markdown export should render as HTML in the new tab instead of plain text

---
