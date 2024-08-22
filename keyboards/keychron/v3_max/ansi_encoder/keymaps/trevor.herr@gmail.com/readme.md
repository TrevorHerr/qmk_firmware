# Compile Custom Keymap

Setup QMK MSYS if required pointing it to the `wireless_playground` branch of this repo:

```
qmk setup -H <repo_path>
```

Full environment setup documentation: https://docs.qmk.fm/newbs_getting_started

Set the default keyboard to `keychron/v3_max/ansi_encoder`:

```
qmk config user.keyboard=keychron/v3_max/ansi_encoder
```

Compile the keymap:

```
qmk compile -b keychron/v3_max/ansi_encoder -m trevor.herr@gmail.com
```

Flash the compiled firmware. Put the v3 max into DFU (Bootloader) Mode by holding down the `esc` key while plugging in the keyboard: https://docs.qmk.fm/newbs_flashing
