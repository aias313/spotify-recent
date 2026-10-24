# Brag plan: Recently Played

## Rubric
- **What is it:** A one-page web tool that turns your last Spotify plays into a playlist.
- **Who / what for:** Anyone who just had a great listening run and wants to keep it. Three taps on a phone.
- **What sets it apart:** No app, no server, no secret. Runs entirely in the browser on GitHub Pages with Spotify's PKCE flow.
- **Most impressive claim:** Last 50 plays → playlist in three taps. Range and bulk-select in between.
- **Visual hook:** The page's own dark UI with the green accent; a phone fills with tracks like a receipt printing.
- **Real UI shown:** Header, Connect button, range chips, the track list with checkboxes, the selection counter, the name field, the "Playlist created" card. Rebuilt from the page's actual CSS and markup.
- **Tone:** `default` — punchy, playful, clean.
- **Share caption:** Turned my last 50 Spotify plays into a playlist in three taps. No app, no server, just a page.

## Privacy
Track names and artists in the video are fictional stand-ins (no real listening history). No Client ID or tokens appear on screen.

## Identity (from index.html, dark theme)
- bg #121613 · surface #1b211d · fg #eef2ec · muted #94a098 · line #2b332d · accent #3ac46f · accent-fg #0d1a11 · accent-soft #1b3324
- Display: Archivo 800, tight tracking. Body: Inter Tight.

## Music
120 BPM, 4/4 → 0.5 s/beat, 2 s/bar. 21 s = 10.5 bars. Every cut lands on a beat. Kick on 1 and 3, hat on 8ths, bass + soft pad in A minor; a short click SFX on each cut and a two-note "ding" on the playlist-created beat, all in key and quantized to the grid.

## Storyboard (1920×1080, 30 fps, 21 s)
| # | Time | Scene | On screen | Motion | Cut |
|---|---|---|---|---|---|
| 1 | 0.0–3.0 | Hook | "What were you just listening to?" huge Archivo, left-aligned. | Words land one per beat; a thin accent rule draws under on beat 4. | hard cut on 3.0 |
| 2 | 3.0–7.0 | Reveal | Phone (390 wide, scaled) with the real header; "Connect Spotify" button. Caption right: "Recently Played" + "Your last 50 plays, one tap away." | Simulated tap at 3.5s; tracks print in 8ths from 4.0s (12 rows). | soft push on 7.0 |
| 3 | 7.0–11.0 | Range | Range chips card in focus. | "How many" chips 20→50 (7.5s), "Played within" Any time→Today (9.0s); list reflows. Caption: "Pick the range." | soft push on 11.0 |
| 4 | 11.0–15.0 | Select | Track list with checkboxes; counter "20 of 20 selected". | Tap None (11.5s) → all dim; press-and-hold sweeps rows 3–9 green (12.5–13.5s); counter ticks to "7 of 20 selected". Caption: "Pick the tracks." | soft push on 15.0 |
| 5 | 15.0–18.0 | Name & create | Bottom bar: name field + Create button. | Types "Saturday cleaning" (15–16.5s), button press 17.0s, "Playlist created" card slides up 17.5s with ding. Caption: "Name it. Done." | dip to bg on 18.0 |
| 6 | 18.0–21.0 | Outro | "Recently Played" big; under it the URL `aias313.github.io/spotify-recent`; small line "Runs in your browser. No server. No secret." | Title snaps in on 18.0, URL on 18.5, tag on 19.0; hold. | end |
