- set_hwclock function disabled by default (SETLOCALRTC=0) because it's possible to set hwclock to UTC on Windows through registry
- dell_hwmod function disabled because i8kutils is no more supported

**Firefox VAAPI enabler:
sudo dnf install https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm https://download1.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm
sudo dnf install libva-intel-driver ffmpeg

about:config
media.ffmpeg.vaapi.enabled = true
media.rdd-process.enabled = false
gfx.x11-egl.force-enabled = true
