# agri-quiz-keepawake

Free keep-awake pinger for the AGRI QUIZ DAILY EXAM SYSTEM runner.

The runner is a Render **free** web service (`engine/web.py` in the private repo `b9811507-del/live-test`).
Render free instances sleep after 15 minutes without traffic, so this workflow pings
`https://live-test-8wu1.onrender.com/ping` every 5 minutes. Each run also prints the runner's status
JSON (cycles, last runs, next test slot) into the log, so the Actions tab doubles as an uptime page.

* Public repository → GitHub Actions minutes are **free and unlimited** here.
* No third-party account, no credit card, no VM.
* If the Render service is renamed, update `RUNNER_URL` in `.github/workflows/keepawake.yml`.
