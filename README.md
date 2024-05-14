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
### google-chrome
> 应用商店->设置->开启AUR
```
# 需要先安装其它依赖包
sudo pacman -S fakeroot

# 在商店搜索google-chrome，选中并完成安装
```