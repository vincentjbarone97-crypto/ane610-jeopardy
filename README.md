# ANE610 Jeopardy (GitHub Pages Ready)

A standalone, browser-based Jeopardy study game for ANE610. No React build required — it’s a single `index.html` that loads a JSON question set.

## Quick Start (GitHub Pages)

1. Create a new GitHub repository (public or private).
2. Upload **all files** in this folder (`index.html`, the `questions/` folder).
3. Go to **Settings → Pages**:
   - **Source:** Deploy from a branch
   - **Branch:** `main` (or `master`) • **Folder:** `/root`
   - Click **Save**. Wait ~30–60s for deployment.
4. Open your site at: `https://<your-username>.github.io/<repo-name>/`

### Using the Game
- Open the site, click **Load Questions (JSON)**, choose `questions/ANE610_Jeopardy_Game.json` (or any JSON file with the same schema).
- Set team count/names → **Reset** → play.
- Daily Doubles + Final Jeopardy included.

## JSON Schema

```json
{
  "title": "ANE610 Exam 1 Review – Jeopardy",
  "categories": [
    {
      "name": "Category Name",
      "clues": [
        {"value": 100, "clue": "Question text", "answer": "Answer text"}
      ]
    }
  ],
  "finalJeopardy": {"category": "Topic", "clue": "Final Q", "answer": "Final A"}
}
```

## Tips
- Add more sets: drop additional files into `questions/` and load them via the button in-app.
- You can also keep everything in one JSON; the app supports 6+ categories.
- To update the board title, edit `"title"` inside your JSON.

## Local Testing (optional)
Just double-click `index.html` — it runs locally in your browser (Chrome/Safari/etc.).

---

Enjoy and good luck on Exam 1!