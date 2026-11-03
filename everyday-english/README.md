# Everyday English — permanent live app
Permanent URL: https://cndbsgh413-alt.github.io/cncncncn/everyday-english/

## Daily card updates
Use the GitHub connector on repository cndbsgh413-alt/cncncncn, branch main.
Read and update ONLY everyday-english/cards.json. Use fetch_file and update_file with its current SHA.
Never replace index.html merely to add expressions.
JSON schema: {"version":"YYYY-MM-DD","cards":[{"id":"unique-id","en":"American English phrase","ko":"한국어 뜻","day":"YYYY-MM-DD","tag":"교실 영어"}]}.
Preserve all earlier card IDs, preserve all cards, deduplicate normalized English text and IDs.
Add only expressions genuinely practiced or corrected with the user in English lessons. Prefer elementary classroom English.
On launch the app syncs JSON with a cache-busting fetch, every five minutes while open, or manual button.
Study records remain in browser localStorage everyday-english-progress-v1.
The repository is public; do not add identifying or sensitive personal information to cards.
A separate ChatGPT scheduled task checks new daily phrases and appends them where accessible.
