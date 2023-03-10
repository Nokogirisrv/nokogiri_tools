<p align="center">
 <img src="https://miro.medium.com/max/1400/1*CdjOgfolLt_GNJYBzI-1QQ.jpeg"width="900"/></a>
</p>

### 1. Update your server.
```
sudo apt update && sudo apt upgrade -y
```
```
sudo apt install make clang pkg-config libssl-dev libclang-dev build-essential git curl ntp jq llvm tmux htop screen unzip cmake -y
```
### 2. If you installing Golang "Go" on clear server you need input following commands.
The latest release of Golang "Go" you can find in this [link](https://go.dev/dl/)
```
wget https://golang.org/dl/go1.19.5.linux-amd64.tar.gz
sudo tar -C /usr/local -xzf go1.19.5.linux-amd64.tar.gz
```
```
cat <<EOF >> ~/.profile
export GOROOT=/usr/local/go
export GOPATH=$HOME/go
export GO111MODULE=on
export PATH=$PATH:/usr/local/go/bin:$HOME/go/bin
EOF
source ~/.profile
go version
sudo rm -rf go1.19.5.linux-amd64.tar.gz
```
### 3. If you would like update your Golang "Go" you need input following commands.
```
sudo rm -rvf /usr/local/go/
```
```
sudo rm -rvf go
```
Than proceed to the [step 2](https://github.com/CryptoSailors/Tools/tree/main/Install%20Golang%20%22Go%22#2-if-you-installing-golang-go-on-clear-server-you-need-input-following-commands) of this guide.
### 4. If you would like delete your Golang "Go" from your server you need input following commands.
```
sudo rm -rvf /usr/local/go/
```
```
sudo rm -rvf go
```