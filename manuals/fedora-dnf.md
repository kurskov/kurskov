dnf в Fedora можно подстроить: https://russianfedora.github.io/FAQ/administration.html  

### установка драйвера nvidia
```
sudo dnf -y install akmod-nvidia
```
### аппаратное декодирование/кодирование видео на видеокарте Nvidia
```
sudo dnf -y install libva-vdpau-driver
sudo dnf -y install mesa-vdpau-drivers
```
### активация поддержки VDPAU при её отсутствии в драйвере (бекенд VA-API для VDPAU, поддерживается только H.264)
```
sudo dnf -y install libvdpau-va-gl
```
### информация о поддержке vdpau в системе
```
sudo dnf -y install vdpauinfo
```
### пакеты с набором библиотек CUDA (Nvidia)-1 пакет подтянет все нужные
```
sudo dnf -y install xorg-x11-drv-nvidia-cuda
```
### подключаем Flatpak в Fedora - и кол-во прилжений зашкаливает:  
```
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
```
