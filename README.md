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

Open freqtrade repository to read
    https://www.freqtrade.io/en/stable/installation/#install-code

Install necessary dependencies
# update repository
sudo apt-get update

# install packages
sudo apt install -y python3-pip python3-venv python3-dev python3-pandas git curl

# Download `develop` branch of freqtrade repository
git clone https://github.com/freqtrade/freqtrade.git

# Enter downloaded directory
cd freqtrade

# your choice (1): novice user
git checkout stable