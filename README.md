<h2 align=center>Gensyn Testnet Node Guide</h2>

## 💻 System Requirements

| Requirement                        | Details                                                                                      |
|-------------------------------------|---------------------------------------------------------------------------------------------|
| **CPU Architecture**                | `arm64` or `amd64`                                                                          |
| **Recommended RAM**                 | 16 GB                                                                                       |
| **CUDA Devices (Recommended)**      | `RTX 3090`, `RTX 4090`, `A100`, `H100`                                                      |
| **Python Version**                  | Python >= 3.10 (For Mac, you may need to upgrade) 


## 🌐 Rent GPU
- Visit : [Quick Pod Website](https://console.quickpod.io?affiliate=64e0d2b2-59ee-4989-a05f-f4c3b6dbb2e4)
- Sign Up using email address
- Go to your email and verify your Quick Pod account
- Click on `Add` button in the corner to deposit fund
- You can deposit using crypto currency (from metamask) or using Credit card
- Now go to `template` section and then select `Ubuntu 22.04 jammy` in the below
- Now click on `Select GPU` and search `RTX 4090` and choose it
- Now choose a GPU and click on `Create POD` button
- Your GPU server will be deployed soon
- Now click on `Connect` option and then choose `Connect to web terminal`

## 📥 Installation

1. **Install `sudo`**
```bash
sudo apt install -y python3 python3-venv python3-pip curl screen git yarn
```
2. **Install other dependencies**
```bash
curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
```
3. **Install Node.js and npm if not installed already**  
```bash
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
```
4. **Clone this repository**
```bash
sudo apt update && sudo apt install -y yarn

5. **Create a `screen` session**
```bash
curl -sSL https://raw.githubusercontent.com/zunxbt/installation/main/node.sh | bash
```
6. **Install Node.js and npm if not installed already**  
```bash
rm -rf rl-swarm && git clone https://github.com/zunxbt/rl-swarm.git && cd rl-swarm

7. **Clone this repository**
```bash
screen -S gensyn

8. **Create a `screen` session**
```bash
python3 -m venv .venv && source .venv/bin/activate && ./run_rl_swarm.sh
```
- It will ask some questions, you should send response properly
- ```Would you like to connect to the Testnet? [Y/n]``` : Write `Y`
- ```Would you like to push models you train in the RL swarm to the Hugging Face Hub? [y/N]``` : Write `N`
- When you will see interface like this, you can detach from this screen session


9. **Detach from `screen session`**
- Use `Ctrl + A` and then press `D` to detach from this screen session.

When you see 'use_cache True setup will complete.
save your node name

Leader board : https://dashboard.gensyn.ai

fore recheck command:
1.cd ~/rl-swarm
1.1. screen -r gensyn
 rerun command:
2. python3 -m venv .venv && source .venv/bin/activate && ./run_rl_swarm.sh
