# Compile Custom Keymap

Change the directory to the qmk_framework repo:

```sh
cd <path>/qmk_firmware
```

Setup QMK MSYS if required pointing it to the `wireless_playground` branch of the repo:

```sh
qmk setup -H <repo_path>
```

Full environment setup documentation: https://docs.qmk.fm/newbs_getting_started

Set the default keyboard to `keychron/v3_max/ansi_encoder`:

```sh
qmk config user.keyboard=keychron/v3_max/ansi_encoder
```

Compile the keymap:

```sh
qmk compile -kb keychron/v3_max/ansi_encoder -km trevor.herr@gmail.com
```

Flash the compiled firmware. Put the v3 max into DFU (Bootloader) Mode by holding down the `esc` key while plugging in the keyboard: https://docs.qmk.fm/newbs_flashing
