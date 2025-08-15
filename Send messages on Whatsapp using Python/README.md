# Send WhatsApp Messages with Python

Quickly send WhatsApp messages (text or images) right from Python. Choose instant delivery or schedule a message for later, and watch it send via WhatsApp Web in your default browser.

## Features

- Send instant text messages
- Send images with an optional caption
- Schedule messages for a specific time (24-hour format)
- Simple prompts and a file picker for images

## Requirements

- Python 3.x
- Jupyter Notebook
- pywhatkit
- tkinter (usually included with Python)
- A default browser logged into WhatsApp Web

Install dependency:
```bash
pip install pywhatkit
```

## Usage

1. Open `Send_whatsapp_messages.ipynb` in Jupyter Notebook.
2. Make sure you are logged into https://web.whatsapp.com/ in your default browser.
3. Run the notebook and choose the message type:
   - `1` = Instant message (optionally attach an image)
   - `2` = Timed (scheduled) message
4. Enter the recipient phone number in full international format, e.g. `+1234567890`.
5. Enter the message text.
6. For images: choose `y` when prompted and select an image file.
7. For scheduled messages: enter Hour (24h) and Minutes when prompted.
8. Keep your browser open; the script will open a tab and send the message automatically.

## Notes

- WhatsApp Web must remain open and logged in for sending to work.
- For scheduled messages, keep your computer awake and connected to the internet.
- Phone numbers must include the country code (E.164 format). Example: `+1...`, `+44...`, etc.
- pywhatkit may briefly bring the browser to the foreground to complete sending.

---

Automate your WhatsApp messages in minutes!
