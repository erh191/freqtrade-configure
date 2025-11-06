# freqtrade-configure
how to download and install freqtrade

How to download this repository.
- Download and install VSCode.
- Open new vscode window.
- Open new terminal. Terminal/New Terminal
- Posicionate in the workspace: 
    cd C:\repos\erh
- Clone this repository: 
    git clone https://github.com/erh191/freqtrade-configure.git
- Open repository folder: click in file/Open folder C:\repos\erh\freqtrade-configure

How to install Ubuntu on WSL
- Donwnload and Install WSL (Windows Subsystem for Linux)
- List Ubuntu in vscode cmd terminal.
     wsl --list --online
- Install last ubuntu with custom name
    wsl --install -d Ubuntu-24.04 --name Ubuntu-24.04-ft
- Set user and password.
- Go to the ubuntu user workspace
     cd /home/erh

How to run Ubuntu from terminal
wsl -d Ubuntu-24.04-ft

Open freqtrade repository to read
    https://www.freqtrade.io/en/stable/installation/#install-code

Install necessary dependencies
# update Ubuntu
sudo apt-get update

# install packages
sudo apt install -y python3-pip python3-venv python3-dev python3-pandas git curl

# Download `develop` branch of freqtrade repository
git clone https://github.com/freqtrade/freqtrade.git

# Enter downloaded directory
cd freqtrade

# your choice: novice user
git checkout stable

Use /setup.sh -install
In Ubuntu, freqtrade provides the script to install freqtrade.
# --install, Install freqtrade from scratch
./setup.sh -i 

Activate your virtual environment¶
Each time you open a new terminal, you must run source .venv/bin/activate to activate your virtual environment.
# activate virtual environment
source ./.venv/bin/activate

You are now ready to run the bot.

# Verify compatible exchanges
 freqtrade list-exchanges -a

# Configure your bot
Read https://www.freqtrade.io/en/stable/configuration/ and excecute:
freqtrade new-config --config user_data/config.json
