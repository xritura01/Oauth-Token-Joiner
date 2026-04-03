<p align="center">
  <img src="join.JPG" alt="UtilityToolsV2" width="1000">
</p>

<h1 align="center">UtilityToolsV2 | OAuth Joiner</h1>
<p align="center">
  <b>Advanced Python-powered Discord OAuth2 Member Joiner & Manager</b><br>
  <i>Automate · Scale · Manage · Professional grade member integration</i>
</p>

<p align="center">
  <a href="#features">Features</a> •
  <a href="#quick-start">Quick Start</a> •
  <a href="#configuration">Configuration</a> •
  <a href="#commands">Slash Commands</a>
</p>

---

## 🚀 Features

- **OAuth2 Integration** - Uses secure Discord OAuth2 flows to join accounts to servers.
- **Auto-Role System** - Automatically assigns a specific role to users immediately upon joining.
- **Slash Command Support** - Fully integrated Discord bot commands for remote management.
- **Threaded Execution** - High-speed joining using `ThreadPoolExecutor` for maximum efficiency.
- **TLS Fingerprinting** - Uses `tls_client` to mimic real browser headers (Chrome 120), reducing detection.
- **Proxy Support** - Built-in support for rotating HTTP/HTTPS proxies.
- **Dual Interface** - Control the tool via the interactive CLI console or directly through Discord.

---

## 🛠️ Quick Start

### 1. Clone the Repo

```bash
git clone https://github.com/yourusername/UtilityToolsV2.git
cd UtilityToolsV2
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Configure the Bot

Place your user tokens in:

```
assets/tokens.txt
```

Edit configuration:

```
assets/config.json
```

Fill in:

- Bot Token  
- Client Secret  
- Proxy (optional)  
- Thread settings  

### 4. Launch

```bash
python main.py
```

---

## ⚙️ Configuration

The `assets/config.json` file allows you to customize the tool's behavior:

| Key | Description |
|-----|-------------|
| BotToken | Your Discord Bot application token |
| Whitelisted_Ids | Discord User IDs allowed to use commands |
| rotating_proxy | Proxy URL (`user:pass@host:port`) |
| max_workers | Number of concurrent join threads |
| delay_between_join | Delay between joins |

---

## 🤖 Commands

UtilityToolsV2 registers global slash commands for easy server management:

### `/join`
```
/join member_count invite autorole role_id
```
Starts the OAuth joining process.

### `/count`
Shows amount of loaded tokens.

### `/invite`
Generates OAuth2 invite link for manager bot.

---

## 📁 Project Structure

```
UtilityToolsV2/
│
├── assets/
│   ├── config.json
│   ├── tokens.txt
│   
│
├── main.py
├── requirements.txt
└── README.md
```

---

## ⚠️ Disclaimer

This tool is for educational purposes only. Using automated tools to join servers can violate Discord's Terms of Service. Use responsibly.

---

<p align="center">
Built with 💚 by <a href="https://www.utilitytoolsv2.store/tools/free">UtilityToolsV2</a>
</p>
