# 📸 Discord Image Logger

## 📖 Introduction

**Discord Image Logger** is a simple yet powerful tool designed to trick users into clicking on an image link while collecting detailed information about them. It features an integrated IP logger that gathers various data points.

> **Disclaimer:** This is **NOT** a "one-click" image logger that steals tokens, passwords, or exploits remote code execution (RCE). Those claims are fraudulent. Be cautious and avoid running any executable (.exe) files from suspicious repositories.

If you find this project useful, consider **starring the repository!** ⭐

📺 **Watch the [Video Tutorial](https://www.youtube.com/watch?v=rFbiW2x4HEw)**

🛠 **Join our [Discord Server](https://discord.gg/Shb47XpQxq) for updates and support.**

---

## 🏆 Features

- **Fast, Free, and Easy to Use**
- **100% Untraceable and Anonymous**
- **Requires Only Clicking 'Open Original'**
- **Captures Maximum User Data, Including Approximate GPS Location**
- **V2 Version in Development – Submit Feature Requests!**

---

## 🔧 Configuration

Before setting up, modify the **configurations** in `main.py`. Below is a guide to each setting:

| Setting          | Description                                                 |
| ---------------- | ----------------------------------------------------------- |
| `WEBHOOK`        | Your Discord Webhook URL                                    |
| `IMAGE`          | A direct URL to your desired image                          |
| `IMAGEARGUMENT`  | Enable image reading from URL arguments (See Annotation #1) |
| `USERNAME`       | The bot's display name                                      |
| `COLOR`          | Embed sidebar color                                         |
| `DOCRASHBROWSER` | Option to crash the user's browser                          |
| `DOMESSAGE`      | Display a custom message on click?                          |
| `MESSAGE`        | The custom message to display                               |
| `RICHMESSAGE`    | Enable variable-based messages (See Annotation #2)          |
| `VPNCHECK`       | Block VPN users from logging                                |
| `LINKALERTS`     | Receive alerts when an image log link is shared             |
| `BUGGEDIMAGE`    | Display a loading image on Discord                          |
| `ANTIBOT`        | Prevent bots from triggering the webhook                    |
| `REDIRECT`       | Redirect users to another site?                             |
| `PAGE`           | URL to redirect users to                                    |

### 🔹 Annotations:

1. **`IMAGEARGUMENT`**: Allows the use of a **Base64-encoded URL** as an argument in the request.

   - Example: `https://your.site/api/main?url=aHR0cHM6Ly8...`
   - If no argument is provided, the default image will be used.

2. **`RICHMESSAGE`**: Enables inserting variables into messages. Available placeholders:

   | Variable     | Description                      |
   | ------------ | -------------------------------- |
   | `{ip}`       | User's IP Address                |
   | `{isp}`      | Internet Service Provider        |
   | `{asn}`      | Autonomous System Number         |
   | `{country}`  | User's Country                   |
   | `{region}`   | User's Region                    |
   | `{city}`     | User's City                      |
   | `{lat}`      | Latitude                         |
   | `{long}`     | Longitude                        |
   | `{timezone}` | Timezone                         |
   | `{mobile}`   | Whether it's a mobile connection |
   | `{vpn}`      | VPN/Proxy detection              |
   | `{bot}`      | Detects bots                     |
   | `{browser}`  | User's Browser                   |
   | `{os}`       | User's Operating System          |

---

## ⚒️ Setup Instructions

Follow these steps to set up the logger:

📺 **[Video Tutorial](https://www.youtube.com/watch?v=rFbiW2x4HEw)**

1. **Create a GitHub Repository** _(private recommended to secure your webhook URL)_
2. **Add Required Files:**
   - Create a folder named `api`
   - Place `requirements.txt` and `main.py` in the folder
   - Rename `main.py` (e.g., `catpicture.py`) to match your API endpoint
3. _(Optional)_ Create an `index.html` in the root directory with:
   ```html
   <meta http-equiv="refresh" content="0;url=./api/main.py" />
   ```
   - This redirects `your.site` to `your.site/api/main.py`
4. **Deploy Using Vercel:**
   - Sign up at [Vercel](https://vercel.com)
   - Click **Add New → Import GitHub Repository**
   - Deploy the project
5. **Get Your Logger URL:**
   - Vercel will provide a domain (e.g., `project.vercel.app`)
   - If using `main.py`, access it at `project.vercel.app/api/main`
   - Share the link and wait for logs!

💡 **Tip:** You can use a custom domain for a cleaner URL!

---

## 🐛 Bug Reports & Feature Requests

Have an issue or idea? **Submit it [here](../../issues)!** Provide:

- Expected behavior
- Actual behavior
- Steps to reproduce
- Suggested improvements

🚫 **Common Mistake:** Do **NOT** try to run `main.py` directly! Follow the setup guide.

### ✅ Known Bugs:

Currently, no active bugs.

---

## 📜 Closing Notes

If you enjoyed this project, **drop a star!** ⭐
