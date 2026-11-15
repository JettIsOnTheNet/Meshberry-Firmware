# Install guide

## Which file

| File | Use it for |
|---|---|
| `MeshBerry-<version>-TLoRaPager-SX1262-full.bin` | First install: Launcher, or USB at address `0x0` |
| `MeshBerry-<version>-TLoRaPager-SX1262-update.bin` | Updating over USB at address `0x10000`, keeping your data |

They are in [`firmware/`](../firmware/). Checksums for verification are provided in `SHA256SUMS`.

Check back of your pager or order page for the radio type! This build is for **SX1262** units!

## Option 1 – Launcher, from the SD card

Use this if your pager already runs [Launcher](https://github.com/bmorcelli/Launcher).

1. Format a microSD card as FAT32, 32 GB or smaller, MBR partition table.
2. Copy `-full.bin` onto the SD card.
3. Put card in the pager and start Launcher.
4. Open SD card file list, pick file and choose to install it.
5. Pager restarts into MeshBerry.

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

3. In Launcher open OTA menu and choose **MeshBerry** from favourites. Launcher's own documentation has the details for your version.

## Option 3 – USB

### First install

This erases everything, including anything previous firmware stored in flash.

1. Connect by USB-C. If it is not detected, hold **BOOT** button while plugging in.
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