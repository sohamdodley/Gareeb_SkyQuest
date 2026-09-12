# SkyQuest Lite (Android Chrome)

Cadet flight game for phones. South Asia + Europe. Ten stages.
One column, large buttons, no Plotly.

## GitHub → Streamlit Cloud

1. Create a **new** GitHub repository.
2. Upload **these files at the repo root** (do not nest another folder):

```
app.py
requirements.txt
README.md
LICENSE
.gitignore
cities.json
stages.json
aircraft.json
.streamlit/config.toml
```

3. Push to `main`.
4. [share.streamlit.io](https://share.streamlit.io) → New app
   - repository: this repo
   - branch: `main`
   - main file: `app.py`
5. Deploy. On the phone open only the `https://….streamlit.app` URL.

First load after sleep can take 1–2 minutes. Leave the tab open.

## Local

```bash
pip install -r requirements.txt
streamlit run app.py
```

## Notes

- Game data is also embedded in `app.py`, so missing JSON will not crash Cloud.
- Progress is session-only.
- This package is the phone build. It is not the desktop dual-view app.
