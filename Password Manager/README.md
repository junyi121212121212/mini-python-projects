# Password Manager

A simple, local password manager you can run from a Jupyter notebook. Add website credentials and have the password encrypted before it’s saved to disk.

## Features

- Add credentials (website, username, password)
- Encrypts passwords using Fernet (symmetric encryption)
- Stores entries in a local `passwords.csv`
- Retrieve and decrypt a saved password (same session)
- Minimal, menu-driven prompts

## Requirements

- Python 3.x
- Jupyter Notebook
- `cryptography`

Install dependency:
```bash
pip install cryptography
```

## Usage

1. Open `password_manager.ipynb` in Jupyter Notebook.
2. Run the cells to start the menu.
3. Choose an option:
   - `1` Add Password
   - `2` Get Password
   - `3` Exit
4. Follow the prompts to enter website, username, and password.
5. Entries are appended to `passwords.csv` in this folder.

## Files

- `password_manager.ipynb` — the interactive notebook UI
- `passwords.csv` — saved entries (website, username, encrypted password)

## Notes & Tips

- Key/session note: The notebook generates a new encryption key each time it runs. That means you can decrypt passwords you add during the same notebook session. After restarting the notebook/kernel, previously saved passwords cannot be decrypted by the newly generated key.
  - If you want persistence across sessions, consider modifying the notebook to generate a key once and save/load it from a file (e.g., `key.key`).
- This is a learning/demo tool, not a production-grade password manager.
- Keep your `passwords.csv` (and any saved key) private.

---

Keep your credentials organized—locally and simply!
