# Install guide

## Which file

First choose a firmware. They do the same things and keep their data in the same place, so you can move from one to the other later.

| Firmware | Files start with | What it is |
|---|---|---|
| [Meshberry and Mesherola](MESHBERRY-MESHEROLA.md) | `MeshBerry-` | The two dot-matrix pager styles, both in one firmware |
| [MeshBerry Bold 9000](BOLD-9000.md) | `MeshBerryBold-` | The colour firmware, with the map and colour emoji |

Then the file for the job (the names below are the dot-matrix ones; the colour firmware's are the same with `MeshBerryBold-` at the front):

| File | Use it for |
|---|---|
| `MeshBerry-<version>-TLoRaPager-SX1262-full.bin` | First install: Launcher, or USB at address `0x0` |
| `MeshBerry-<version>-TLoRaPager-SX1262-update.bin` | Updating over USB at address `0x10000`, keeping your data |

They are in [`firmware/`](../firmware/), with checksums in `SHA256SUMS`.

Check the back of your pager or its order page for the radio type. This build is for **SX1262** units.

## Option 1 – Launcher, from the SD card

Use this if your pager already runs [Launcher](https://github.com/bmorcelli/Launcher).

1. Format a microSD card as FAT32 (32 GB or smaller, MBR partition table).
2. Copy the `-full.bin` file onto the card.
3. Put the card in the pager and start Launcher.
4. Open the SD card file list, pick the file and choose to install it.
5. The pager restarts into MeshBerry.

If Launcher refuses the full file, try the `-update.bin` file the same way.

## Option 2 – Launcher, by link

Launcher can keep download links as favourites and install straight from them over WiFi.

1. In Launcher, connect to WiFi.
2. Open Launcher's `config.conf` on the SD card (or through its web interface) and add an entry to the `"favorite"` list:

```json
{
  "name": "MeshBerry",
  "fid": "",
  "link": "https://github.com/JettIsOnTheNet/MeshBerry-Firmware/raw/main/firmware/MeshBerry-latest-TLoRaPager-SX1262-full.bin"
}
```

3. In Launcher open the OTA menu and choose **MeshBerry** from the favourites. Launcher's own documentation has the details for your version.

## Option 3 – USB

### First install

This erases the pager, including anything a previous firmware stored in flash.

1. Connect the pager by USB-C. If it is not detected, hold the **BOOT** button while plugging in.
2. With [esptool](https://docs.espressif.com/projects/esptool/):

```
esptool.py --chip esp32s3 write_flash 0x0 MeshBerry-<version>-TLoRaPager-SX1262-full.bin
```

A browser flasher that lets you pick a file and an address works too: choose the `-full.bin` file and address `0x0`.

3. Unplug and plug back in, or press reset.

### Update, keeping your data

```
esptool.py --chip esp32s3 write_flash 0x10000 MeshBerry-<version>-TLoRaPager-SX1262-update.bin
```

## First start

1. The dot-matrix firmware starts in the Meshberry style and asks which **style** you want. You can change it later under Device → Style in the settings. (MeshBerry Bold 9000 has one style and skips this.)
2. It asks for your **region**. Pick the one that matches your local mesh; frequency, bandwidth and spreading factor are set for you.
3. It asks for a **name**, whether to **advertise** yourself to the mesh, and whether to **share your GPS position**. Both can be changed later and both can stay off. If you skip these questions, the pager does not advertise: nobody can add you or message you privately until you turn *Advertise* on under *Options → LoRa Radio*.
4. If no SD card is in, you will see *NO SD CARD: USING FLASH*. Everything works; your data is just kept inside the pager instead.

## Going back

To return to another firmware, flash it the same way you flashed this one. If you installed through Launcher, Launcher is still there: see its documentation for how to reach it at start-up.
