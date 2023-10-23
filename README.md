# Ubuntu22.04.3LTS
## Preparacion de Ubuntu con Herramientas Ofensivas
```
sudo apt update & sudo apt upgrade -y
```

```
sudo apt install wireshark -y
```
```
sudo apt install tshark -y
sudo apt install nmap -y
sudo apt install git -y
sudo apt install python3-scapy -y
sudo apt-get install hping3 -y
sudo apt-get install yersinia -y
sudo apt-get install tcpreplay -y
sudo apt install hashcat -y
sudo apt install hydra -y
sudo apt install onesixtyone -y
sudo apt install crunch -y
sudo apt-get install john -y
sudo apt-get install cewl -y
sudo apt install python3-pip -y
sudo apt install terminator -y
sudo apt-get install zsh -y
sudo apt-get install net-tools -y
sudo apt-get install openssh-server -y
sudo apt install curl
```

### Descarga de BurpSuite
https://portswigger.net/burp/releases#community
```
chmod +x burpsuite_community_linux_v2023_10_2_2.sh 
./burpsuite_community_linux_v2023_10_2_2.sh
```
### Descarga de Herramientas GitHub
```
cd
cd Desktop
mkdir tools
cd tools
git clone https://github.com/mkbrutusproject/MKBRUTUS.git
git clone https://github.com/BasuCert/WinboxPoC.git
git clone https://github.com/theevilbit/ciscot7.git
git clone https://github.com/lesandcl/Llaitun.git
```
### Instalacion de ohmyzh
```
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
### Instalacion de Powerlevel10k
```
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```

### Configuracion del tema
```
sed -i 's/ZSH_THEME="robbyrussell"/ZSH_THEME="powerlevel10k\/powerlevel10k"/' ~/.zshrc
```
### Instalacion de plugins de zsh
```
sudo apt install zsh-autosuggestions
sudo apt install zsh-syntax-highlighting
```

### Configuracion de plugins
```
echo "#Plugins" >> ~/.zshrc
echo "source /usr/share/zsh-autosuggestions/zsh-autosuggestions.zsh" >> ~/.zshrc
echo "source /usr/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> ~/.zshrc
```
### Descarga e instalacion de fonts Powerlevel10k
```
wget https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Regular.ttf
wget https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold.ttf
wget https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Italic.ttf
wget https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold%20Italic.ttf
sudo mv MesloLGS\ NF\ *.ttf /usr/local/share/fonts/
fc-cache -fv
```

> [!NOTE]
> Se debe reiniciar y configurar las fonts en terminator

### Instalacion de versiones anteriores de python
```
sudo apt install software-properties-common -y
sudo add-apt-repository ppa:deadsnakes/ppa -y
sudo apt update
sudo apt install python3.7 -y
sudo apt install python3.7-distutils -y
cd /usr/lib/x86_64-linux-gnu/
sudo ln -s -f libc.a liblibc.a
```

```
sudo apt install virtualenv -y
```
### Instalacion de requerimientos de Llaitun y ejecucion
```
cd Llaitun
pip install -r requirements.txt
sudo $(which python) Llaitun.py 
```

### Instalacion de ambiente virtual
```
cd
cd Desktop/tools/
virtualenv env3.7 -p python3.7
source env3.7/bin/activate
```
### Cambio de Fondo de pantalla
```
cd
cd Pictures
wget https://getwallpapers.com/wallpaper/full/4/e/5/724440-free-download-ubuntu-wallpaper-hd-1920x1080.jpg
gsettings set org.gnome.desktop.background picture-uri "file://$(pwd)/724440-free-download-ubuntu-wallpaper-hd-1920x1080.jpg"
```
### Instalacion de Obsidian
Descarga https://obsidian.md/download
```
sudo apt-get install fuse -y
```
```
chmod u+x Obsidian.AppImage
```
```
./Obsidian-1.0.3.AppImage --disable-gpu
```
