# Fedora

sudo dnf update
sudo dnf install sddm
sudo systemctl enable sddm
sudo systemctl set-default graphical.target
sudo dnf install git
git clone https://github.com/christitustech/fedora-titus
git clone https://github.com/pisojap/fedora
mkdir .config
cp fedora-titus/bg.jpg .config/
cp -r fedora-titus/dotconfig/bspwm .config/
sudo dnf install vim
cp -r fedora-titus/dotconfig/polybar .config/
cp -r fedora-titus/dotconfig/kitty .config/
cp -r fedora-titus/dotconfig/picom.conf .config/
cp -r fedora-titus/dotconfig/sxhkd .config/
cp -r fedora-titus/dotconfig/Thunar .config/
sudo dnf install bspwm dconf-editor kitty picom polybar rofi sxhkd thunar
cp -r ../fedora-titus/dotconfig/rofi .config/
cd ..
cp fedora-titus/.x* ~
cp fedora-titus/.X* ~
sudo dnf install nitrogen
sudo dnf install ./fedora-titus/rpm-packages/ocs-url-3.1.0-1.fc20.x86_64.rpm 
sudo vim /etc/sddm.conf #set session to bspwm and user to cephaspi
reboot
sudo dnf install fontawesome-fonts fontawesome-fonts-web
sudo dnf install firefox
sudo dnf install arandr
cd Downloads/
mkdir ~/.fonts
mv * ~/.fonts/
cd ~/.fonts/
unzip FiraCode.zip 
unzip Meslo.zip 
rm *.zip
fc-cache -vf
sudo dnf install neofetch
