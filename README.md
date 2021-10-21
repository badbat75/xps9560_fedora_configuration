Firefox VAAPI enabler:
dnf install https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm https://download1.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm
dnf install libva-intel-driver ffmpeg

about:config
media.ffmpeg.vaapi.enabled = true
media.rdd-process.enabled = false
gfx.x11-egl.force-enabled = true