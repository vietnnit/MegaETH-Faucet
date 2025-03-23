# ⚡ MegaETH Faucet Script

Welcome to the **MegaETH Faucet Script** – a powerful, multi-threaded tool that automates MegaETH token claims using 2Captcha and proxies.

> 🛠️ Easy to set up, blazing fast, and highly customizable.

---

## 🌟 Features

- 🚀 Multi-threaded execution (high throughput)
- 🤖 Automatic Turnstile captcha solving using 2Captcha
- 🌐 Proxy support for enhanced anonymity
- 🧾 Log results to success/fail files
- 🪄 Retry mechanism to increase claim success rate
- 📊 Real-time logging with colorful CLI output

---

## 🧰 Installation Guide

### 🐧 For Linux/macOS

1. **Clone the repository**
```bash
git clone https://github.com/RPCHubs/MegaETH-Faucet.git
cd MegaETH-Faucet
```

2. **Install Python dependencies**
```bash
pip install -r requirements.txt
```

3. **Configure the script**
- Open `faucet.py`
- Go to **line 14–15** and edit the following:
```python
THREADS = 100  # Set number of threads (e.g., 100–500)
TWO_CAPTCHA_API_KEY = "your-2captcha-api-key"  # Replace with your 2Captcha API key
```

4. **Run the script**
```bash
python3 faucet.py
```

---

### 🪟 For Windows

1. **Clone the repository**
```powershell
git clone https://github.com/RPCHubs/MegaETH-Faucet.git
cd MegaETH-Faucet
```

2. **Install Python dependencies**
```powershell
pip install -r requirements.txt
```

3. **Edit the configuration**
- Open `faucet.py` in a code editor
- Go to **line 14–15**:
```python
THREADS = 100
TWO_CAPTCHA_API_KEY = "your-2captcha-api-key"
```
- Replace with your desired values

4. **Execute the script**
```powershell
python faucet.py
```

---

## 📁 Required Files

Make sure these files exist in the same directory:

- `wallets.txt` – 💼 List of wallet addresses (one per line)
- `proxies.txt` – 🌐 List of HTTP proxies in format: `http://user:pass@ip:port`

Optional Output:
- `success.txt` – ✅ Wallets that successfully claimed
- `fail.txt` – ❌ Wallets that failed

---

## 🧪 How It Works

1. Loads wallets and proxies
2. Solves Turnstile Captcha via 2Captcha
3. Sends claim request to MegaETH faucet
4. Logs results with retry mechanism

---

## 📣 Community & Support

Need help or want to connect?

- 🛠️ [RPC Hubs Channel](https://t.me/RPC_Hubs)
- 💬 [RPC Community Chat](https://t.me/chat_RPC_Community)

We're here to support you! 🫶

---

## 🔍 Demo

```bash
# Sample terminal output
[12:01:22 24/03/2025] [1] Claiming for address: 0x123...
[12:01:25 24/03/2025] [1] Turnstile solved OK
[12:01:27 24/03/2025] [1] Claim SUCCESS for wallet 0x123...
```

---

Made with ❤️ by the RPC Hubs Team

