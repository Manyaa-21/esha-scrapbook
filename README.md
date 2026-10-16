# Somewhere Between Us — Esha's scrapbook ♡

A mobile-friendly, flip-through friendship scrapbook book with layered paper, washi tape, faux binder rings, page-turn animations, eight sprinkled photo frames, editable lore, five emotional letters, an original Ahmedabad → UIUC mini arcade game, voice recording/audio upload, and a six-question quiz.

## How the flip-through book works
The website is now arranged as one topic per page: cover, memories, lore, five letters, Ahmedabad → UIUC race, voice notes, friendship quiz, final letter, and back cover. Use **previous / next** at the bottom, tap the top navigation links, or use the left/right arrow keys on a keyboard. The page controls also work on mobile.

## Preview locally
Open `index.html` in a browser. You can edit most text directly by clicking it. Photo picker previews are temporary and local to your browser; for photos that Esha can see on the published site, follow the permanent-photo steps below.

## Make photos permanent
1. Create a folder named `photos` beside `index.html`.
2. Put your chosen pictures there, e.g. `photos/esha-01.jpg`.
3. In the matching photo frame, replace the placeholder `<span>` and temporary `<img id="i1" hidden>` with `<img src="photos/esha-01.jpg" alt="Us being ridiculous">`. Repeat for each frame. Resize/compress large photos for mobile data.

## Add a permanent voice note
Record or upload a voice note, download it, and put the file in a folder named `audio`. Add an audio player where you want it, e.g. `<audio controls src="audio/for-esha.mp3"></audio>`. Browser recordings are not automatically saved to the repository. Microphone recording normally requires HTTPS or localhost.

## Personalize the letters and lore
Search in `index.html` for each letter heading, then replace the text inside its `letterbody` element. Lore headings and paragraphs are editable in the page, but those edits are not saved back to the file automatically: copy them into `index.html` before publishing. Use exact phrases, nicknames, dates, and tiny details only you two understand.

## Edit the quiz
Each question is a `.quizq` element with `data-answer="2"`. The answer index is zero-based: first choice is 0, second 1, third 2, fourth 3. Change the question, four options, and correct index together. There are six questions already.

## Publish using GitHub Pages
1. On GitHub, click **New repository** and name it `esha-scrapbook`.
2. Choose Public if you want a simple shareable GitHub Pages URL. Do not upload anything private that you would not want others to see.
3. Add/upload `index.html` and `README.md` to the repository root and commit.
4. Open **Settings → Pages**. Under build/deployment, choose **Deploy from a branch**, choose `main` and `/(root)`, then Save.
5. Wait for GitHub to provide the Pages URL (typically `https://YOUR-USERNAME.github.io/esha-scrapbook/`) and open it on a phone before sending it to Esha in India.

This project is static HTML/CSS/JS and needs no build tools. Google Fonts requires internet; system fallbacks are included.
