# Bitz Miner CLI on Eclipse


## Install Dependecies
**1. Install Packages**
```bash
bash <(curl -s https://raw.githubusercontent.com/sadi200/Bitz/refs/heads/main/run1/run.sh)
```
* Close and reopen your Terminal.
```
solana version
```
* If you get `solana: command not found` RUN :
```bash
echo 'export PATH="/root/.local/share/solana/install/active_release/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```
```
solana --version
```

**4. Switch RPC**
```bash
solana config set --url https://bitz-000.eclipserpc.xyz
```

---

## Wallet CLI
### . Create a CLI wallet
```bash
solana-keygen new
```
---

## Install Bitz
```bash
cargo install bitz
```

---

## Run Bitz Miner
### 1. Open a screen

```bash
screen -S bitz
```

### 2. Start Miner
```bash
bitz collect
```

### Usefull Commands

Check account info:
```bash
bitz account
```

link wallet:

```bash
cat ~/.config/solana/id.json
```

Claim Bitz to your Node Wallet:
```bash
bitz claim
```
minimize screen:
  ```bash
  Ctrl+A+D
  ```
ON/OFF: 
```bash
screen -r bitz
 ```
