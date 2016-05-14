# Raspberry Pi - VGA over HDMI output

A simpe Ansible role to manage VGA output over HDMI on a Raspberry Pi. Tested with the jessie lite raspbian image and a common HDMI to VGA adapter.

After successful provisioning you need to reboot for the changes to take effect

## Role Variables

```` yaml
raspi_hdmi_group: 2
# 0   Auto-detect
# 1   CEA (TVs)
# 2   DMT (Monitors)

raspi_hdmi_mode: 4
# examples for monitors
# 4   640x480
# 16  1024x768
# 85  1280x720
# 82  1920x1080

raspi_display_rotate: 0
# 0        Normal
# 1        90 degrees
# 2        180 degrees
# 3        270 degrees
# 0x10000  horizontal flip
# 0x20000  vertical flip

raspi_audio_over_hdmi: no
````

For detailed options see [the official documentation](https://www.raspberrypi.org/documentation/configuration/config-txt.md).
