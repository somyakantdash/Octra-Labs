# STEP BY STEP Full GUIDE OF OCTRA LABS (in Codespace)

---
# 🪙 TASK 1 : Wallet Created

### 🔹 STEP 1: Open in Codespace

1. Go to - https://github.com/octra-labs/wallet-gen
2. Click the green `Code` button  
3. Select → `Open with Codespaces` → `+ New codespace`
4. Wait for the environment to fully load

---

---

## 🔹 Step 1: Install Bun

```bash
curl -fsSL https://bun.sh/install | bash
source ~/.bashrc
bun --version
````

---

## 🔹 Step 2: Install Dependencies

```bash
bun install
```

---

## 🔹 Step 3: Build the Project

```bash
bun run build
```

---

## 🔹 Step 4: Start the Server

```bash
bun start
```

> ✅ After this, click the **“PORTS”** tab in Codespace and open `localhost:8888` in browser.

---

**Done! Wallet Generator is live. 🔐**


---
# 🪙 TASK 2 : TOKEN TRANSFER

### 🔹 STEP 1: Open in Codespace

1. Go to - [https://github.com/octra-labs/octra_pre_client](https://github.com/octra-labs/octra_pre_client)
2. Click the green `Code` button  
3. Select → `Open with Codespaces` → `+ New codespace`
4. Wait for the environment to fully load

---

### 🔹 STEP 2: Install dependencies

In the Codespace terminal, run:

```bash
pip install -r requirements.txt
````

---

### 🔹 STEP 3: Create and edit wallet.json

Create the wallet file:

```bash
cp wallet.json.example wallet.json
```

Then open the file: wallet.json

Paste your test wallet details (⚠️ never use your real wallet):
![Wallet Generation](IMG_20250630_110429.png)


```
{
  "priv": "private key here",
  "addr": "octxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
  "rpc": "https://octra.network"
}
```

---

### 🔹 STEP 4: Send a test transaction

```bash
python cli.py send --to oct5ziFzQJkiJFPfcQeuAmp4vhfQgjwb8gyx2W2TZdGhzJm --amount 0.01
```

🟢 That’s it! You can now access the wallet UI and make transactions to addresses found on the explorer: https://octrascan.io/

---
