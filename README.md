# h87a-wkl-firmware
Extremely barebones QMK firmware for the hineybush h87a PCB compiled with a 1000 Hz polling rate, asym_eager_defer_pk debounce (at 5 ms), NKRO enabled, and all backlight/RGB underglow features disabled in a standard ANSI WKL TKL keymap.
## Layout
![image](https://user-images.githubusercontent.com/54309603/212494647-b715d43c-b0e2-4bf8-929f-fa52e53b7c6a.png)
## Build options in rules.mk & additions in config.h
```
BOOTMAGIC_ENABLE = no      # Enable Bootmagic Lite
MOUSEKEY_ENABLE = no       # Mouse keys
EXTRAKEY_ENABLE = no       # Audio control and System control
CONSOLE_ENABLE = no        # Console for debug
COMMAND_ENABLE = no        # Commands for debug and configuration
NKRO_ENABLE = yes            # Enable N-Key Rollover
BACKLIGHT_ENABLE = no      # Enable keyboard backlight functionality
RGBLIGHT_ENABLE = no       # Enable RGB underglow
AUDIO_ENABLE = no           # Audio output
LTO_ENABLE = yes
DEBOUNCE_TYPE = asym_eager_defer_pk
```
```
#define USB_POLLING_INTERVAL_MS 1
#define FORCE_NKRO
```
