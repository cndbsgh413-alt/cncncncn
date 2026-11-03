# My Natural English — live flashcards

Permanent GitHub Pages URL: https://cndbsgh413-alt.github.io/cncncncn/english/

- **Never replace index.html for routine new phrases.** Update only `english/cards.json` on the `main` branch.
- JSON schema: `{ "version":"YYYY-MM-DD", "cards": [{"id":"d6-01", "en":"...", "ko":"...", "day":"YYYY-MM-DD", "tag":"교실 영어"}] }`.
- Preserve every existing card ID and all existing cards. Only append deduplicated new phrases (normalized English text); use unique stable IDs.
- After an English conversation finishes, add that session's corrected classroom English and conversational American expressions to this JSON by GitHub connector `fetch_file` then `update_file` with the returned current blob SHA.
- On opening the app, `index.html` fetches `./cards.json` with cache busting. It rechecks when the user returns to the page and every 5 minutes while open. The `↻ 최신 표현 확인` button triggers a refresh.
- Learning progress is kept in the browser's `localStorage` under `my-american-english-flashcards-v1`. Do not reset or rename this key; existing progress must remain.
- For devices moving from an old URL/origin, the user must do a **one-time** backup in the old app and restore in the new one.
- Public GitHub Pages means the expressions can be viewed publicly; don't include names or sensitive personal details in cards.
