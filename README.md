# Selah Journal

A private, faith-informed journal for Android and the web.

- Entries and photos are encrypted on your device (AES-256) before they reach Google Drive.
- Passphrase: opens the journal on a new device or computer. If it's lost, entries can't be recovered.
- PIN: daily unlock on each device. Five wrong tries removes that device's copy (Drive copy stays).
- Prompts send only your chosen focus and the "About me" note to Claude. Reflections send only the entry you choose.

## Setup
1. Google Cloud Console: create a project, enable the Google Drive API, set up the OAuth consent screen (External, add yourself as a test user), and create an OAuth client ID of type "Web application" with authorized JavaScript origin `https://YOUR-USERNAME.github.io`.
2. Paste the client ID into `CONFIG.GOOGLE_CLIENT_ID` at the top of the script in `index.html`.
3. Upload all files to a new GitHub repo and turn on GitHub Pages.
4. Open the site in Chrome on your phone, then use "Add to Home screen" / "Install app".
5. In the app's Settings, paste a Claude API key from console.anthropic.com.
