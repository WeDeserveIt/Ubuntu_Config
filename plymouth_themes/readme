//开机动画

把解压后的文件夹复制到 "/usr/share/plymouth/themes/" 文件夹下

sudo ln -s /usr/share/plymouth/themes/deb10/deb10.plymouth /etc/alternatives/default.plymouth
sudo ln -s /etc/alternatives/default.plymouth /usr/share/plymouth/themes/deb10/default.plymouth //如果这个不设置关机动画不正常
//重新生成 initramfs 镜像
sudo update-initramfs -u

sudo gedit /etc/alternatives/default.plymouth
//修改最后两行，如果正确则不用修改
[script]
ImageDir=/usr/share/plymouth/themes/${theme-directory}
ScriptFile=/usr/share/plymouth/themes/${theme-directory}/${script-file-name}
