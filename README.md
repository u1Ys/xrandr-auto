# xrandr-auto
Wrapper of `xradnr` to automatically complement output information

## Examples

When the primary ouput is `eDP-1` and external ouput `HDMI-1` with
maximum size 1920x1080...

`xrandr-auto ...` = `xrandr --output HDMI-1 ...`

`xrandr-auto _max ...` = `xrandr --output HDMI-1 --mode 1920x1080 ...`

`xrandr-auto ... _primary` = `xrandr --output HDMI-1 ... eDP-1`

`xrandr-auto _max --right-of _primary` = `xrandr --output HDMI-1 --mode 1920x1080 --right-of eDP-1`
