# manjaro.desktop

## 常用tools
### ifconfig
```
pacman -S net-tools
```

### docker
```
sudo pacman -S docker

# 开机自启
sudo  systemctl enable docker

# 使你的账号运行docker命令无需root
sudo usermod -aG docker youraccount
```