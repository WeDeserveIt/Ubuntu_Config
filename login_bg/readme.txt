sudo cp ${picture-path} /usr/share/backgrounds/

sudo gedit /etc/alternatives/gdm3.css

[change the following segment] 

#lockDialogGroup {

    background: #2c001e url(resource:///org/gnome/shell/theme/noise-texture.png);

    background-repeat: repeat; }

==>

#lockDialogGroup {

    background: #2c001e url(file:///usr/share/backgrounds/壁纸名称);

    background-repeat: no-repeat;

    background-size: cover;

    background-position: center; }

