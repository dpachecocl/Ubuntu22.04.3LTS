# Ubuntu22.04.3LTS
Preparacion de Ubuntu

``sudo apt install wireshark -y``
`sudo apt install tshark -y`
`sudo apt install nmap -y`
sudo apt install git -y
sudo apt install python3-scapy
sudo apt install hashcat -y
sudo apt install hydra -y
sudo apt install onesixtyone -y
sudo apt install crunch -y
sudo apt-get install john -y
sudo apt-get install cewl -y
sudo apt install python3-pip -y
sudo apt install terminator -y
sudo apt-get install zsh -y
sudo apt install curl
`

##Descarga de BurpSuite
chmod +x burpsuite_community_linux_v2023_10_2_2.sh 
./burpsuite_community_linux_v2023_10_2_2.sh

git clone https://github.com/mkbrutusproject/MKBRUTUS.git
git clone https://github.com/BasuCert/WinboxPoC.git
git clone https://github.com/theevilbit/ciscot7.git

sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k

sed -i 's/ZSH_THEME="robbyrussell"/ZSH_THEME="powerlevel10k\/powerlevel10k"/' ~/.zshrc

sudo apt install zsh-autosuggestions
sudo apt install zsh-syntax-highlighting

echo "#Plugins" >> ~/.zshrc
echo "source /usr/share/zsh-autosuggestions/zsh-autosuggestions.zsh" >> ~/.zshrc
echo "source /usr/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> ~/.zshrc

wget https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Regular.ttf
wget https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold.ttf
wget https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Italic.ttf
wget https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold%20Italic.ttf
sudo mv MesloLGS\ NF\ *.ttf /usr/local/share/fonts/
fc-cache -fv

sudo apt install software-properties-common -y
sudo add-apt-repository ppa:deadsnakes/ppa -y
sudo apt update
sudo apt install python3.7
sudo apt install python3.7-distutils
cd /usr/lib/x86_64-linux-gnu/
sudo ln -s -f libc.a liblibc.a
