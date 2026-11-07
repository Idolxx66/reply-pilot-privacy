# Privacy Policy — Reply Pilot for Etsy

**Last updated: November 3, 2026**

Reply Pilot for Etsy ("the extension") is a Chrome extension that generates AI reply drafts inside the Etsy seller inbox. This policy explains exactly what happens to your data. The short version: **we have no servers and collect nothing.**

## 1. What the extension stores

The extension stores the following settings using `chrome.storage.sync` (Google Chrome's built-in settings sync, bound to your Google account):

- Your AI provider API key (e.g., DeepSeek or OpenAI)
- API endpoint URL and model name
- Your preferred reply tone
- Your shop rules / policies text

These settings never leave Chrome's sync storage. The developer has no access to them.

## 2. What data leaves your browser, and where it goes

When you click "AI Reply Draft":

- The text of the currently visible Etsy conversation is read from the page.
- That conversation text is sent **directly from your browser to the AI API endpoint that YOU configured** (default: DeepSeek at api.deepseek.com) along with your tone and shop rules, to generate a reply draft.
- The generated draft is displayed to you locally. It is inserted into the reply box only when you click "Insert".

Your conversation text is governed by the privacy policy of the AI provider you choose (DeepSeek, OpenAI, etc.). We recommend reviewing your provider's data policy.

## 3. What the extension does NOT do

- Does NOT send any data to servers operated by the developer (we operate none).
- Does NOT collect, transmit, or sell personal information, browsing history, or analytics.
- Does NOT send messages automatically. Every reply is reviewed and sent by you.
- Does NOT access any website other than Etsy seller message pages (host permission: `*.etsy.com`).
- Does NOT contain remote code, trackers, or third-party scripts.

## 4. Permissions justification

| Permission | Why |
|---|---|
| `storage` | Save your API key and preferences locally |
| `https://*.etsy.com/*` | Inject the draft button and read conversation text on Etsy seller message pages only |

## 5. Data retention and deletion

All settings live in `chrome.storage.sync`. Uninstalling the extension removes them. There is no server-side data to delete because no server-side data exists.

## 6. Changes to this policy

If this policy changes, the updated version will be published at the same URL with a new "last updated" date.

## 7. Contact

Questions about this policy: open an issue at the project's GitHub repository or use the Support tab on the Chrome Web Store listing.
