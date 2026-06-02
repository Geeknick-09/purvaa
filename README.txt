For Purva 💗 — Standalone Bundle
================================

Files in this zip
-----------------
  index.html          → the website
  assets/music.mp3    → the background song
  assets/proposal.mp4 → the proposal scene video

IMPORTANT: keep the "assets" folder right next to index.html.
The HTML loads music and video using the relative paths
"assets/music.mp3" and "assets/proposal.mp4". If you rename
or move the folder, the audio/video will not play.

----------------------------------------------------------
HOW TO UPLOAD TO A HOSTING PROVIDER
----------------------------------------------------------

Option A — Netlify Drop (easiest, free, ~30 seconds)
  1. Go to https://app.netlify.com/drop
  2. Drag the WHOLE unzipped folder (containing index.html
     AND the assets folder) onto the page.
  3. You instantly get a public URL like
     https://something-random.netlify.app
  4. Open it on your phone / share the link.

Option B — Vercel
  1. Go to https://vercel.com/new
  2. Choose "Deploy" → upload the folder, or drag-and-drop.
  3. Done — you get a public URL.

Option C — GitHub Pages
  1. Create a new GitHub repo.
  2. Upload index.html and the assets folder (keep the structure).
  3. Repo Settings → Pages → Source: "main" branch, root.
  4. Wait ~1 minute, open the URL Pages shows you.

Option D — cPanel / shared hosting / your own server
  1. Open File Manager (or use FTP / FileZilla).
  2. Go into your public_html (or www) folder.
  3. Upload index.html AND the entire assets folder together.
     Make sure the structure on the server is:
         public_html/index.html
         public_html/assets/music.mp3
         public_html/assets/proposal.mp4
  4. Visit your domain.

----------------------------------------------------------
WHY THE AUDIO MIGHT GO SILENT (and how to avoid it)
----------------------------------------------------------

1. Forgetting to upload the "assets" folder.
   → Always upload index.html AND assets/ together.

2. Renaming files. The HTML expects exactly:
        assets/music.mp3
        assets/proposal.mp4
   Do not rename them. If you do, also update the src= in index.html.

3. Browser autoplay policy.
   Modern browsers block sound until the user interacts with
   the page. This site is already designed for that: the music
   starts on the first scroll/tap, and swells when the gift is
   opened. Just tell Purva to scroll — she does not need to
   press anything.

4. HTTPS vs HTTP.
   Use an HTTPS URL (Netlify, Vercel, GitHub Pages all give
   HTTPS automatically). Some browsers block media on plain HTTP.

5. Mobile silent switch.
   If the phone is on silent / vibrate mode, the music will
   not play out loud. Ring mode + volume up = best experience.

Enjoy. ❤️
