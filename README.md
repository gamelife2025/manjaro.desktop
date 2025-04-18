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

### 触摸板手势
> see:https://github.com/bulletmark/libinput-gestures
1. 安装依赖项
```
sudo pacman -S xdotool
```
2. 使用AUR安装此软件  
链接:https://aur.archlinux.org/packages/libinput-gestures
3. 配置权限
```
sudo gpasswd -a $USER input
```
4. 自启动
```
libinput-gestures-setup autostart start
```
5. 配置  
```
# vim ~/.config/libinput-gestures.conf
# 三指上滑 切换窗口
gesture swipe up 3 xdotool key ctrl+F10
```
6. 重启
