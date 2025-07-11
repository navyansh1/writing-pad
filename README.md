# GuardNote
GuardNote is a secure, privacy-focused digital notebook that runs entirely in your browser. It uses your own private GitHub Gists for optional cloud synchronization, ensuring your notes remain completely under your control.

**Live Demo:** [**https://guardnote.vercel.app**](https://guardnote.vercel.app)

## Features

*   **Privacy-First Sync:** Securely sync your notes across devices using your private GitHub Gists. You control the access token and your data never touches a third-party server.
*   **Local-First Operation:** All notes are saved in your browser's local storage by default. Cloud sync is entirely optional.
*   **Rich Drawing Tools:** Includes a resizable pen, an adjustable eraser, and multiple color options for a natural writing experience.
*   **Unlimited Notebooks & Pages:** Organize your thoughts in separate notebooks, each with as many pages as you need.
*   **Customizable Page Styles:** Choose between plain, ruled, or grid paper to suit your needs.
*   **PDF Export:** Save and share an entire notebook as a single, portable PDF file.
*   **No Tracking:** Zero analytics, cookies, or data collection. Your notes are for your eyes only.
*   **Responsive Design:** Works seamlessly on desktops, tablets, and mobile devices.

## How to Use

### Local Usage
Simply open the `index.html` file (or visit the [live demo](https://navyansh1.github.io/writing-pad/)) in your browser. All your notes will be saved locally on your device.

### Setting Up Cloud Sync

To sync your notes securely across multiple devices, you can link GuardNote to your GitHub account.

1.  **Generate a GitHub Token:**
    *   Navigate to [GitHub's Personal Access Tokens (classic)](https://github.com/settings/tokens/new) page.
    *   Give your token a descriptive name (e.g., "GuardNote Sync").
    *   Set an expiration date for the token.
    *   Under `Select scopes`, check the box next to **`gist`**. No other permissions are required.
    *   Click **Generate token** and copy the new token immediately.

2.  **Configure GuardNote:**
    *   In the GuardNote app, click the **`🔑 Setup`** button in the header.
    *   A prompt will appear. Choose option `1` to set up cloud sync.
    *   Paste the GitHub token you just created and click OK.

3.  **Sync Your Notes:**
    *   **To Save:** To save your current notebooks to the cloud, click the **`☁️ Sync`** button. This will create a new private Gist in your GitHub account or update an existing one.
    *   **To Load on a New Device:**
        1.  On your primary device (where notes are saved), go to `🔑 Setup` and select option `3` to get your unique sync code (Gist ID).
        2.  On your new device, go to `🔑 Setup`, select option `2`, and enter the sync code.
        3.  Click the **`📥 Load`** button to pull your notes from the cloud.
