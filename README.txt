ENT321 — 30‑Minute Quiz (Offline web app)
Files included:
- ent321-quiz.html
- style.css
- logo.svg
- questions.json
- answers.csv
- README.txt

How to open locally (quick):
1. Put all files in a single folder (e.g., ent321-quiz).
2. Open ent321-quiz.html in your browser (double-click). The app will try to load questions.json; if the browser blocks local fetch, the embedded fallback will be used.

Recommended: run a simple static server (ensures fetch works):
- Python 3:
  cd ent321-quiz
  python -m http.server 8000
  Then open http://localhost:8000/ent321-quiz.html

Features:
- 30-minute countdown timer (auto-submits when time runs out).
- Randomized question order and shuffled options each run.
- Progress indicator and per-question navigation.
- Review screen after submission showing correct answers and your answers.
- Restart quiz button to retake.
- Download results as CSV (student results).
- Instructor answer key included in answers.csv.

answers.csv:
- Contains mapping of question number to correct letter and correct option text.
- Use this file for grading or instructor reference.

If you want:
- A packaged ZIP file ready to download (I provided file contents here so you can create the ZIP locally).
- A small Node/Express backend to record results (I can provide code).
- A version that posts results to a Google Sheet (requires credentials).

To create the ZIP locally (macOS / Linux):
cd ent321-quiz
zip -r ../ent321-quiz.zip *

Windows PowerShell:
Compress-Archive -Path .\* -DestinationPath ..\ent321-quiz.zip

Enjoy — ENT321 quiz ready to run.
