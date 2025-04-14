# 🧠 Dria Compute Node Guide

This guide walks you through the process of installing and running a Dria Compute Node on **Linux**, **macOS**, or **Windows**.

---

## ⚙️ Installation

❌ **Do NOT use WSL if you're not on Linux.**  
Use native OS or follow the correct steps for Windows.

---

### 🐧 Step-by-Step for **Linux / macOS**:

1. Open your terminal
2. Run the command below to install the Dria launcher:

```bash
curl -fsSL https://dria.co/launcher | bash
```

---

### 🪟 Step-by-Step for **Windows**:

1. Open **PowerShell** as **Administrator**
2. Run the following command:

```powershell
powershell -c "irm https://dria.co/launcher.ps1 | iex"
```

3. 🔁 **Restart PowerShell** after running the above command.

---

## 🚀 Starting Your Dria Node

Once installed, you'll need to start your node and provide:

- Your **EVM private key** (without the `0x`)
- The **Model(s)** you want to run

---

### 🐧 On **Linux / macOS**:

```bash
sudo dkn-compute-launcher start
```

---

### 🪟 On **Windows**:

```powershell
dkn-compute-launcher.exe start
```

---

## 🎁 Enter Referral Code to Earn Extra Steps (Points)

To earn bonus rewards, enter a referral code:

```bash
sudo dkn-compute-launcher referrals
```

Use the arrow keys to select:  
**"Enter referral code to be referred"**

Then enter this code:

```text
zyL643oVtFgQqACsqFRV
```

You can use referral codes from other users too.

---

## ✅ Final Steps

- After entering the referral code, go back and **start your node**.
- You can **check your node status** here:  
  [https://dria.co/edge-ai](https://dria.co/edge-ai) (Enter your wallet address)

- **Get your Discord Role** by filling this form:  
  [Discord Role Form](https://form.typeform.com/to/Eav42hR3?typeform-source=www.google.com)

- **Join the Telegram channel** for updates:  
  [Crypto Income Free Telegram](https://t.me/cryptoincomefree)

---

## 🛡️ Tips for Security

- **Never** share your **EVM private key**
- Use a dedicated wallet, and run only on a secure device
- Ensure a stable internet connection for best performance

---

## 🔗 Useful Links

- 🌐 [Dria Website](https://dria.co/)
- 💾 [Download Ollama](https://ollama.com/download/linux)
- 💬 [Join Dria Discord](https://discord.gg/driacompute)

---

## 🙋 Support

- Join the [Dria Discord](https://discord.gg/driacompute)
- Open an issue on this repo if something isn’t working
- DM the community mods in Telegram if you're stuck

---

**Happy computing, and may your node earn well!**
---

## 🔁 Switching Model Backend: Ollama to Gemini API

This guide is especially useful if:

- Your device cannot run Ollama
- Ollama is not working properly on your system

---

### 🛑 Step 1: Stop Your Node

If your node is currently running, stop it before proceeding.

---

### 🧹 Step 2: Delete Existing Dria Config

#### 🔺 On **Linux / macOS**:

```bash
sudo rm -rf .dria
```

#### 🔺 On **Windows (PowerShell)**:

```powershell
Remove-Item -Path "$HOME\Downloads\launcher.ps1", "$HOME\AppData\Local\Temp\launcher.ps1" -Force -ErrorAction SilentlyContinue
```

---

### ♻️ Step 3: Reinstall the Dria Launcher

Follow the same steps from the installation section above to reinstall the launcher for your OS.

---

### 🚀 Step 4: Start the Node and Choose Gemini

```bash
sudo dkn-compute-launcher start
```

- During setup, **choose Gemini** instead of Ollama
- Then enter your **Gemini API Key**

You can get a free Gemini API key here:  
[https://aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey)

---

### ✅ You're Done!

Your node is now running using the Gemini backend instead of Ollama.  
This setup works even on low-spec devices!

**Let’s goooo!** 🚀✅
