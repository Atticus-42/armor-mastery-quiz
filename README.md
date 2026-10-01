# Armor Operations Mastery Quiz

A free, browser-based practice aid for the *Fundamentals of Armor Operations* lesson. Students enter a name, confirm the study warning, and take a 25-question Easy, Medium, or Hard examination at https://atticus-42.github.io/armor-mastery-quiz/. Questions are reshuffled on every attempt.

Questions use only the substantive pages 13-83 of the supplied presentation (fundamentals, characteristics, mechanized infantry, cavalry, tank operations, planning considerations and major equipment). Instructor profile, classroom rules, safety, objectives, icebreaker and administration slides are excluded. Scenarios are fictional Philippine Army situations grounded in those pages.

No login, payment, analytics, cookies, advertising, external fonts, images, scripts or runtime libraries. Answers stay in browser memory. Only the name, difficulty, score and finish time are sent to the class history Google Sheet (tab "Armor History") through `HISTORY_ENDPOINT` in `src/template.html`.

`src/questions/` holds the three banks, `src/template.html` is the page source, and `scripts/build.mjs` produces the self-contained `index.html`. `apps-script/Code.gs` is the shared history web app (one spreadsheet, one tab per lesson). Test gate:

```sh
node scripts/build.mjs && node scripts/verify.mjs
```
