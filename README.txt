Garden Board PWA package

Files included:
- index.html
- manifest.webmanifest
- sw.js
- icons/
- a_digital_watercolor_style_background_illustration.png

Before uploading:
1. Open index.html
2. Replace REPLACE_WITH_YOUR_PUBLIC_ANON_OR_PUBLISHABLE_KEY with your Supabase public anon key
3. Upload the full contents of this folder to your GitHub Pages site root

If you have not already done so, run this SQL in Supabase:
alter table tasks
add column if not exists archived boolean default false;

alter table tasks
add column if not exists archived_at timestamp with time zone;


Voice integration:
- Tap the microphone button in quick add.
- On supported browsers, speech will fill the quick add box.
- Review if needed, then tap + to add.
- iPhone/iPad Safari supports speech recognition with partial support / prefixed behavior.
