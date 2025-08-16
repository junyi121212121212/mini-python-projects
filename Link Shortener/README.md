# Link Shortener

Quickly shorten long URLs into clean bit.ly links using the Bitly API from a simple Jupyter notebook.

## Features

- Convert any long URL to a Bitly short link
- Uses Bitly API v4 with a personal access token
- Reads your token from a local `.env` file (no hardcoding)
- Minimal, prompt-driven flow

## Requirements

- Python 3.x
- Jupyter Notebook
- `requests`
- `python-dotenv`

Install dependencies:
```bash
pip install requests python-dotenv
```

## Bitly Account & API Setup (2–3 minutes)

1. Create a free Bitly account at https://bitly.com/ (or sign in).
2. Generate a Personal Access Token (Bitly API v4):
   - In Bitly, go to Settings (Profile) > Developer Settings > API
   - Create a token (aka "Generic Access Token" or "Access Token").
3. Create a `.env` file in this folder with your token:
   ```
   BITLY_API_KEY=your_bitly_access_token_here
   ```

Keep this token private. Anyone with it can use your Bitly account.

## Usage

1. Open `web_link_shortener.ipynb` in Jupyter Notebook.
2. Run the cells.
3. When prompted, paste the long URL you want to shorten.
4. The notebook will print your Bitly short link (e.g., `https://bit.ly/...`).

## How It Works

- Loads environment variables from `.env` via `python-dotenv`.
- Sends a POST request to `https://api-ssl.bitly.com/v4/shorten` with your long URL.
- Uses the header `Authorization: Bearer <your token>`.
- On HTTP 200, prints the returned `link` field (your short link).

## Notes & Tips

- If you see an error, double-check that your `BITLY_API_KEY` is valid and not expired.
- Bitly free plans have rate limits/quotas.
- You can customize domains or groups with additional Bitly API parameters if needed.

---

Shorten links in seconds with a tiny notebook and Bitly!
