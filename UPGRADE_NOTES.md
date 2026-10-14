# Voice of Goila 2.0 - first upgrade build

- Existing hero text, existing color variables, CMS/data integrations, admin, submission, PWA and APK assets retained.
- Hero image: assets/goila-drone.webp (supplied by project owner).
- Existing category cards now navigate to category.html?section=SLUG.
- Blood donation card moves to coaching/home tutor card position and is visually featured.
- Category pages reuse existing app logic and data.

## Testing
Serve the folder locally using `python3 -m http.server 8000` then open http://localhost:8000. Check Supabase-backed content in deployed preview with correct credentials and policies.

## Known limits
Category routes use a shared category.html page with distinct query-string URLs. The category subcategory details still use the original modal logic within that category page. No backend schema or privacy policy was changed. Existing service worker cache may delay updates after deployment; verify cache behavior.
