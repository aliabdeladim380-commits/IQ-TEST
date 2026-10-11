# Mindform Pro v2 — Visual Reasoning Edition

A responsive reasoning quiz built with plain HTML, CSS and JavaScript.

## What's improved

- Five interface languages: English, French, Arabic, Spanish and Chinese. Arabic uses right-to-left layout.
- Question prompts and options are translated separately on demand and cached locally. Option order and the original answer key are never shuffled or changed.
- Ten visual pattern puzzles drawn as crisp inline SVG illustrations, including shape-sequence riddles. Their prompts, shape names and answer labels are localized in all five languages (Arabic uses Arabic letters; Chinese uses 甲/乙/丙/丁).
- No Previous/Next buttons. Choosing an answer automatically advances to the next question; the final question has a clear Finish Level action.
- Level review shows only the selected answer and whether it was right or wrong. It never reveals the correct answer or explanation.
- Passed levels offer Next Level, Retry and All Levels. Failed levels offer Retry, All Levels, and an explicit “Continue anyway” option so you are not stuck if you want to move on. The next level is unlocked when you choose to continue anyway.
- Ten levels, 65 questions, progress indicator, optional 60-minute timer, and responsive mobile styling.

## Run it

1. Extract the ZIP into a folder.
2. Open `index.html` in a modern browser. For the most reliable experience, serve the folder through a local web server or host it as a static website.
3. Choose a language from the selector in the top-right and start the test.

## Translation note

English is the authored source for the non-visual question bank. Other question text is translated one field at a time using the public MyMemory translation endpoint, so an internet connection is needed for first-time translations. Translations are cached in the browser when storage is available. If translation fails, the app shows a localized error and a retry option instead of silently displaying English answer choices. Machine translations can occasionally be imperfect; the answer key remains unchanged.

## Files

- `index.html` — page shell and metadata
- `styles.css` — responsive design and visual puzzle styling
- `script.js` — question bank, scoring, progression, five-language UI, SVG puzzles and translations
