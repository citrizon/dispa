# Dispa
Dispa is a simple system status indicator written in gtkmm 4<br>
![preview](https://github.com/System64fumo/sysvol/blob/main/preview.gif "preview")


# Configuration
Dispa can be configured in 2 ways<br>
1: By changing dispa.conf at `~/.config/dispa/dispa.conf`<br>
2: Using launch arguments<br>
```
Arguments:
  -p	Set position (eg: top, top-left, bottom, right)
  -o	Set orientation (eg: v, h)
  -W	Set window width
  -H	Set window Height
  -i	Set icon size
  -P	Hide percentage
  -m	Set margins ("top right bottom left")
  -t	Set timeout
  -T	Set transition time (0 disables animations)
  -b	Set custom backlight path
  -M	Set things to monitor (audio_in, audio_out, brightness, keyboard)
  -k	Set keyboard path (/dev/input/by-id/my_keyboard-event-kbd)
  -v	Prints version info
```

To use PulseAudio instead of Wireplumber,<br>
change `#define AUDIO_WIREPLUMBER` to `#define AUDIO_PULSEAUDIO` in `src/config.hpp`

# Theming
Dispa uses your gtk4 theme by default, However it can be also load custom css,<br>
Just copy the included style.css file to `~/.config/dispa/style.css`<br>

# Credits
[Jason White](https://gist.github.com/jasonwhite/1df6ee4b5039358701d2) for showing how to write pulseaudio stuff<br>
[waybar](https://github.com/Alexays/Waybar) for showing how to write wireplumber stuff<br>
[Syshud](https://github.com/System64fumo/syshud) for the original project