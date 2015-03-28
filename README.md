# LimelightPiInstaller
Generic RasperryPI installer and configuration script for Limelight 

This is a fork of the Limelight RetroPie+Emulation station installer script for generic install on any Raspian based Pi-system

LimelightInstaller.sh - script is used to install and configure limelight with retropie 

Limelightconfig.sh - script is used to reconfigure ip and keymap settings for limelight without installing stuff again

Howto use:

just drop the LimelightInstaller.sh in to your home directory

chmod +x LimelightInstaller.sh

./LimelightInstaller.sh

After the install just run the resolution/fps corresponding .sh file from the limelight folder and your a go

<hr>

Known issues:

60fps streaming will not work without lag since it needs the h264_freq setting pumped up on the Rasperry pi. To get it working you need to overclock your Pi, here are the settings that worked for me:

arm_freq=1100 core_freq=500 sdram_freq=500 h264_freq=500 over_voltage=8 force_turbo=1 temp_limit=80

DISCLAIMER: Force_turbo will void your warranty since its keeps the clock on 100% without throttling, so you should use a heatsink with these settings. I will not be responsible if your cat catches fire or your pi explodes because of these

<hr>

Special thanks to the Guys from the Possibly Unsafe -youtube channel whose lime light video tutorial sparked the idea to make the install a tad easier. You can follow them here: https://www.youtube.com/channel/UCyvRzvYxTv1Zz0x--GN_Z7w
