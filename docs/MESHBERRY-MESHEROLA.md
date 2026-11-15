# Meshberry and Mesherola

- **Meshberry** – the spiritual sucessor of a BlueBerry 850
- **Mesherola** – the reincarnation of an Oterola T900

## Contents

- [First start](#first-start)
- [Controls](#controls)
- [The main screen](#the-main-screen)
- [Messages](#messages)
- [Channels](#channels)
- [Adding people](#adding-people)
- [Radar](#radar)
- [Message Info, Node Info and Trace Path](#message-info-node-info-and-trace-path)
- [Alerts](#alerts)
- [Screen](#screen)
- [Calendar, tasks and alarm](#calendar-tasks-and-alarm)
- [Date and time](#date-and-time)
- [WiFi](#wifi)
- [Web interface](#web-interface)
- [GPS](#gps)
- [Radio](#radio)
- [Remote admin](#remote-admin)
- [SD card](#sd-card)
- [Phone app](#phone-app)
- [Battery life](#battery-life)

Check out the features, side by side, in the [feature comparison](FEATURES.md).

## First start

| Meshberry | Mesherola |
|---|---|
| ![Start-up: the logo, then how the radio came up, Meshberry](../screenshots/meshberry/boot.png) | ![Start-up: the logo, then how the radio came up, Mesherola](../screenshots/mesherola/boot.png) |

Advertising and position sharing are both off unless you answer *On*. If you skip the questions the pager does not advertise, and nobody can add you or message you privately until you turn *Advertise* on under *Options → LoRa Radio*.

## Controls

| Control | What it does |
|---|---|
| Wheel, turn | Move through lists and menus |
| Wheel, press | Select, or open the menu for the current screen |
| Wheel, hold | In settings: a tip for the setting. In the emoji picker: keep as a favourite |
| Shift + wheel | A screenful at a time. On the main screen: brightness |
| Space + wheel | On the main screen: volume |
| Enter | Same as pressing the wheel; sends a message while typing |
| Shift + Space | The emoji picker, while writing a message |
| BOOT button, short press | Screen off (and, with *Key Lock* on, keys locked) |
| BOOT button, hold 1.5 s | Power off |
| Backspace | Delete; on an empty line and in lists, back |
| Backspace, hold 1.5 s on the main screen | Keyboard light on / off |

### Typing

- Hold either shift key (beside Z or beside M), or hold SPACE, and press a key to type the symbol printed on it.
- Tap shift once for one capital letter. Tap it twice for caps lock; tap again to release.

### Quick brightness and volume

On the main screen, hold **Shift** and turn the wheel for a brightness slider, or hold **Space** and turn it for volume. Turning up gives more. Volume plays a short tick at the new level when you stop turning. The slider goes away by itself a few seconds after the last turn, or at once with any key.

| Meshberry | Mesherola |
|---|---|
| ![Shift + wheel: brightness, Meshberry](../screenshots/meshberry/quick-brightness.png) | ![Shift + wheel: brightness, Mesherola](../screenshots/mesherola/quick-brightness.png) |
| *Shift + wheel: brightness* | |
| ![Space + wheel: volume, Meshberry](../screenshots/meshberry/quick-volume.png) | ![Space + wheel: volume, Mesherola](../screenshots/mesherola/quick-volume.png) |
| *Space + wheel: volume* | |

### Tips

Not sure what a setting does? In any settings list, **hold the wheel** on it (or press **?**) for a short explanation. On the less obvious settings the tip also comes up by itself if you rest on one for a few seconds; turning the wheel carries on to the next setting.

| Meshberry | Mesherola |
|---|---|
| ![A tip, Meshberry](../screenshots/meshberry/tip.png) | ![A tip, Mesherola](../screenshots/mesherola/tip.png) |
| *A tip* | |

### Emoji

While writing a message, press **Shift + Space** for the emoji picker. It takes the whole screen.

| Control | What it does |
|---|---|
| Wheel | One emoji at a time: through the favourites row at the top, then on down the list |
| Shift + wheel | A screenful at a time |
| Space | Jump to the next group (faces, people, animals, food, travel...) |
| Wheel click or Enter | Put the emoji in your message |
| Hold the wheel | Keep the emoji in the favourites row. Held on a favourite: take it out |
| Backspace | Leave without picking |

The favourites row holds as many as fit across the screen. A new favourite goes on the right and the others move left; when the row is full, the oldest one on the left drops off.

These two styles have a set of 23 dot pictures. An emoji they have no picture for shows as a small box (flags show as their two letters), and it is still passed on correctly: the other end sees the real thing.

| Meshberry | Mesherola |
|---|---|
| ![The emoji picker, Meshberry](../screenshots/meshberry/emoji.png) | ![The emoji picker, Mesherola](../screenshots/mesherola/emoji.png) |
| *The emoji picker* | |

### Questions and notices

Anything that asks first (*leave this channel?*) or reports back (*SAVED*) comes up as a box in the middle of the screen. Turn the wheel to pick a button and click; **Y** and **N** answer too, and Back is always *no*.

| Meshberry | Mesherola |
|---|---|
| ![A question: Y, N, or the wheel, Meshberry](../screenshots/meshberry/popup-ask.png) | ![A question: Y, N, or the wheel, Mesherola](../screenshots/mesherola/popup-ask.png) |
| *A question: Y, N, or the wheel* | |
| ![A notice: any key puts it away, Meshberry](../screenshots/meshberry/nfc-saved.png) | ![A notice: any key puts it away, Mesherola](../screenshots/mesherola/nfc-saved.png) |
| *A notice: any key puts it away* | |

### Key Lock

Turn on *Options → Device → Key Lock* and, once your screen has gone off, keyboard and wheel do nothing at all: they do not even light the screen. To get back in, **hold wheel down for 1.1 second**; the screen shows *KEYS LOCKED* and a bar that fills while you do.

| Meshberry | Mesherola |
|---|---|
| ![Unlocking: the bar fills while the wheel is held, Meshberry](../screenshots/meshberry/lock-holding.png) | ![Unlocking: the bar fills while the wheel is held, Mesherola](../screenshots/mesherola/lock-holding.png) |
| *Unlocking: the bar fills while the wheel is held* | |

- A short press of the **BOOT** button turns the screen off straight away, which locks it.
- A message can still light the screen (if *Wake Screen* is on) and an alarm still rings; any key silences the alarm. The screen shows *KEYS LOCKED*, not what is underneath, until you unlock it.
- On USB power the web sign-in number and the *Web Interface* screen show through the lock, so you can sign in from the desk. On the battery they wait for the unlock too.
- Turned face down (*Flip to Mute*), the screen goes dark and quiet at once, but the keys lock only after the usual screen time-out.
- While it is locked the BOOT button does nothing, so a pocket cannot switch the pager off.
- With Key Lock off, nothing changes except that BOOT turns the screen off and any key wakes it.

### Power

- **Off:** hold BOOT, or choose *Power Off* at the bottom of Options (Meshberry) or Preferences (Mesherola). The pager says *HOLD WHEEL TO POWER ON* and switches everything off.
- **On:** hold the wheel or BOOT for about a second. A short bump does nothing, on purpose.
- At 10% it warns once. When the battery is empty it says so and switches itself off cleanly; charge it over USB to bring it back.

## The main screen

| Meshberry | Mesherola |
|---|---|
| ![The main screen, Meshberry](../screenshots/meshberry/home.png) | ![The main screen, Mesherola](../screenshots/mesherola/home.png) |
| *The main screen* | |

Nine entries, the same in every style:

Messages · Compose · Channels · Address Book · Calendar · Tasks · Alarm · Radar · Options (Preferences on Mesherola)

At the top of the screen: the clock, an envelope with the number of unread private messages, a speech bubble with the number of unread channel messages, **W** when WiFi is connected, **B** when a phone is connected, signal bars and battery bars.

| Meshberry | Mesherola |
|---|---|
| ![Options / Preferences: every group of settings, Meshberry](../screenshots/meshberry/options.png) | ![Options / Preferences: every group of settings, Mesherola](../screenshots/mesherola/options.png) |
| *Options / Preferences: every group of settings* | |
| ![Inside one group, Meshberry](../screenshots/meshberry/settings.png) | ![Inside one group, Mesherola](../screenshots/mesherola/settings.png) |
| *Inside one group* | |

## Messages

**Messages** holds private conversations, one row for each person, newest first. Open a row to see the whole conversation, oldest at the top. Type and press Enter to answer; the wheel scrolls back.

| Meshberry | Mesherola |
|---|---|
| ![Messages: one row per person, Meshberry](../screenshots/meshberry/messages.png) | ![Messages: one row per person, Mesherola](../screenshots/mesherola/messages.png) |
| *Messages: one row per person* | |
| ![A conversation, Meshberry](../screenshots/meshberry/conversation.png) | ![A conversation, Mesherola](../screenshots/mesherola/conversation.png) |
| *A conversation* | |
| ![Writing a reply, Meshberry](../screenshots/meshberry/typing.png) | ![Writing a reply, Mesherola](../screenshots/mesherola/typing.png) |
| *Writing a reply* | |
| ![Sent, then delivered, Meshberry](../screenshots/meshberry/sent.png) | ![Sent, then delivered, Mesherola](../screenshots/mesherola/sent.png) |
| *Sent, then delivered* | |

Your latest message shows *[sent]* and then *[delivered]* once the other pager confirms it; one that never got through stays marked *[not delivered]*. With nothing typed, press the wheel for Message Info, Trace Path, Node Info and Delete Conversation.

**Compose** starts a conversation. Pick a person, type, press Enter.

| Meshberry | Mesherola |
|---|---|
| ![Compose: pick who to write to, Meshberry](../screenshots/meshberry/compose-to.png) | ![Compose: pick who to write to, Mesherola](../screenshots/mesherola/compose-to.png) |
| *Compose: pick who to write to* | |
| ![Writing a new message, Meshberry](../screenshots/meshberry/compose.png) | ![Writing a new message, Mesherola](../screenshots/mesherola/compose.png) |
| *Writing a new message* | |

A message can be 160 bytes: plain letters are one each, emoji and accented letters more. On a channel your name travels with the text, so the room is 160 less your name and two.

A private message needs the other person in your address book and you in theirs. See [Adding people](#adding-people).

## Channels

**Channels** lists the Public channel and any you have joined. Inside a channel, type and press Enter to post.

| Meshberry | Mesherola |
|---|---|
| ![Channels, Meshberry](../screenshots/meshberry/channels.png) | ![Channels, Mesherola](../screenshots/mesherola/channels.png) |
| *Channels* | |
| ![The Public channel, Meshberry](../screenshots/meshberry/channel.png) | ![The Public channel, Mesherola](../screenshots/mesherola/channel.png) |
| *The Public channel* | |
| ![The channel menu, Meshberry](../screenshots/meshberry/channel-menu.png) | ![The channel menu, Mesherola](../screenshots/mesherola/channel-menu.png) |
| *The channel menu* | |

- Type `@` to pick a name to mention.
- Press the wheel with nothing typed for the channel menu:
  - **Message a Person** – pick someone who has posted, add them and write to them privately
  - **Message Info** – pick a message and see how it reached you
  - **Sound** – step through ring tones for this channel
  - **Count Unread** – *Yes* or *No*. Set to *No*, this channel's unread messages are left out of the channel count on the main screen (handy for Public or a busy test channel). They still show beside the channel's name in the Channels list
  - **Leave Channel** – on channels you added
- *Add #channel…* joins an open channel by name. The box starts with the `#` already in it, and the name is made lower case: an open channel's key comes from its name, so `#Test` and `#test` would be different channels, and lower case is what the rest of the mesh uses. *Add private channel…* joins one by name and key, or makes a new key if you leave it blank.
- **To leave a channel:** in the Channels list, hold the wheel on it or press **D**, then choose *Leave* in the box that comes up (or press **Y**). Its messages are deleted with it. Public cannot be left.
- In a channel, typing `/key` shows its key; `/leave` leaves it without asking.

## Adding people

| Meshberry | Mesherola |
|---|---|
| ![Address Book, Meshberry](../screenshots/meshberry/address-book.png) | ![Address Book, Mesherola](../screenshots/mesherola/address-book.png) |
| *Address Book* | |

Someone can be added once the pager knows their public key. Four ways:

1. **Advert.** When they advertise, they appear under *Address Book → Discovered*. Nobody is added by themselves: the list holds the last 50 nodes heard, people first, then repeaters, rooms and sensors, and with an SD card it is kept for 30 days. Click to add; the pager says *Added*. If the address book is full (it holds 64) it offers to replace the contact heard longest ago that is not starred. *Advertise me now* sends yours. With *Advertise* switched off it is *Advertise me once*: it asks first, then sends a single advert and leaves the setting off.
2. **From a channel.** Channel menu → *Message a Person*. If their advert has not been heard yet, the pager offers to ask them for one.
3. **QR code.** *Options → Device → Show My QR Code* shows your contact code for the MeshCore phone app to scan.
4. **NFC tag.** *Address Book → Add by NFC tag*. The pager shows *TOUCH NFC TAG TO MESHBERRY*; hold the tag against its back. It tells you what the tag holds - a person, a repeater, a channel - and asks before saving anything (Y and N answer it). *Address Book → Write my NFC tag* puts your own contact on a blank or rewritable tag, for others to scan. The NFC reader is powered only while that screen is up, and gives up by itself after half a minute.

| Meshberry | Mesherola |
|---|---|
| ![Add by NFC tag: waiting for a tag, Meshberry](../screenshots/meshberry/nfc-scan.png) | ![Add by NFC tag: waiting for a tag, Mesherola](../screenshots/mesherola/nfc-scan.png) |
| *Add by NFC tag: waiting for a tag* | |
| ![What the tag held, and the question, Meshberry](../screenshots/meshberry/nfc-found.png) | ![What the tag held, and the question, Mesherola](../screenshots/mesherola/nfc-found.png) |
| *What the tag held, and the question* | |
| ![Write my NFC tag, Meshberry](../screenshots/meshberry/nfc-write.png) | ![Write my NFC tag, Mesherola](../screenshots/mesherola/nfc-write.png) |
| *Write my NFC tag* | |
| ![Written, Meshberry](../screenshots/meshberry/nfc-written.png) | ![Written, Mesherola](../screenshots/mesherola/nfc-written.png) |
| *Written* | |

![Your contact as a QR code](../screenshots/qr-contact-code.png)

Repeaters, room servers and sensors you have added are kept in their own list inside the Address Book. Star the contacts you want to keep for good (*Node Info* menu): a starred contact is never the one replaced when the address book is full.

## Radar

| Meshberry | Mesherola |
|---|---|
| ![Radar, Meshberry](../screenshots/meshberry/radar.png) | ![Radar, Mesherola](../screenshots/mesherola/radar.png) |
| *Radar* | |

Shows every saved or discovered node that shares a position, at its true bearing and distance from you, north up. The wheel steps through them, nearest first; the ring scale adjusts to the selected node. Click opens a saved node. It needs GPS on and a fix.

## Message Info, Node Info and Trace Path

| Meshberry | Mesherola |
|---|---|
| ![Message Info: how a message reached you, Meshberry](../screenshots/meshberry/message-info.png) | ![Message Info: how a message reached you, Mesherola](../screenshots/mesherola/message-info.png) |
| *Message Info: how a message reached you* | |
| ![Node Info, Meshberry](../screenshots/meshberry/node-info.png) | ![Node Info, Mesherola](../screenshots/mesherola/node-info.png) |
| *Node Info* | |
| ![Trace Path: signal at every hop, Meshberry](../screenshots/meshberry/trace.png) | ![Trace Path: signal at every hop, Mesherola](../screenshots/mesherola/trace.png) |
| *Trace Path: signal at every hop* | |

**Message Info** (from a conversation or channel menu) shows when a message arrived, how many repeaters it passed, whether it was flooded or sent along a known path, the signal it was heard at, and the repeaters on the way.

**Node Info** shows a contact's type, the path to it, when it was last heard, its signal, its position if it shares one, and its key. From there you can reset the path, give the person their own ring tone, or remove them.

**Trace Path** sends a packet out along the known path and back, and lists the signal at each repeater.

## Alerts

| Meshberry | Mesherola |
|---|---|
| ![Alerts, Meshberry](../screenshots/meshberry/alerts.png) | ![Alerts, Mesherola](../screenshots/mesherola/alerts.png) |
| *Alerts* | |

*Options → Alerts*

| Setting | Meaning |
|---|---|
| Sound, Tone, Volume | The default ring |
| Vibrate | Buzz on a message |
| Wake Screen | Turn the screen on for a message (off by default, to save battery) |
| Flip to Mute | Lay the pager face down: two quick blips stepping down, then it is silent with the screen off. Pick it up: two stepping up and it is awake. With *Key Lock* on, the keys lock only after the usual screen time-out, not the moment it is turned over |
| Flip Sound | Those blips, on or off |
| Mute Public | No alert for the Public channel |

A person can have their own tone (*Node Info → Sound*), and so can a channel (channel menu → *Sound*). *Silent* is one of the choices.

The tones are played on a pager-style buzzer voice, with a different default for each style.

## Screen

| Meshberry | Mesherola |
|---|---|
| ![Screen settings, Meshberry](../screenshots/meshberry/screen.png) | ![Screen settings, Mesherola](../screenshots/mesherola/screen.png) |
| *Screen settings* | |

*Options → Screen*: brightness, contrast, backlight effect, **Color** (Green, Amber, Blue, White, Red, Pink, Purple, Classic; *Auto* gives each style its own), LCD effect, LCD Streaks (the faint lines along busy rows and columns, on or off), keyboard light level, and screen timeout.

**Dark Screen** turns the display to light dots on dark glass: *Off*, *At night* (between *Dark From* and *Dark Until*) or *Always*. In *At night* the keyboard light follows it: on in the dark, off by day.

| Meshberry | Mesherola |
|---|---|
| ![Dark Screen: the main screen, Meshberry](../screenshots/meshberry/other-home.png) | ![Dark Screen: the main screen, Mesherola](../screenshots/mesherola/other-home.png) |
| *Dark Screen: the main screen* | |
| ![Dark Screen: a channel, Meshberry](../screenshots/meshberry/other-channel.png) | ![Dark Screen: a channel, Mesherola](../screenshots/mesherola/other-channel.png) |
| *Dark Screen: a channel* | |

## Calendar, tasks and alarm

| Meshberry | Mesherola |
|---|---|
| ![Calendar, Meshberry](../screenshots/meshberry/calendar.png) | ![Calendar, Mesherola](../screenshots/mesherola/calendar.png) |
| *Calendar* | |
| ![Tasks, Meshberry](../screenshots/meshberry/tasks.png) | ![Tasks, Mesherola](../screenshots/mesherola/tasks.png) |
| *Tasks* | |
| ![Alarm, Meshberry](../screenshots/meshberry/alarm.png) | ![Alarm, Mesherola](../screenshots/mesherola/alarm.png) |
| *Alarm* | |

**Calendar** is a month on Meshberry and a list of the coming days on Mesherola; open a day to add or read its entries. **Tasks** is a checklist: click to tick one off.

**Alarm** rings once a day at the time you set. *Ring While Muted* lets it ring even when Sound is off or the pager is flipped face down. Any key silences it.

## Date and time

*Options → Date/Time*: set the time and date by hand, choose a **Clock** of 12 or 24 hours (every time on the pager follows it, and you can type times either way: `19:05` or `7:05p`), and your zone.

**Time from GPS** sets the clock from the satellites. It only does anything while GPS is switched on (*Options → GPS*) and has a fix; the row says *GPS off* when it is waiting for that. Indoors, with no fix, the clock is left alone. The clock keeps running from the pager's own clock chip in between.

## WiFi

| Meshberry | Mesherola |
|---|---|
| ![WiFi, Meshberry](../screenshots/meshberry/wifi.png) | ![WiFi, Mesherola](../screenshots/mesherola/wifi.png) |
| *WiFi* | |
| ![Check for Update, Meshberry](../screenshots/meshberry/update.png) |  |
| *Check for Update* | |

*Options → WiFi*. The pager remembers up to ten networks: **Add a Network** scans, you pick one and type its password. **Saved Networks** lists them; click one to forget it or to change whether the web interface starts by itself there.

| WiFi | What it does |
|---|---|
| Off | Radio off |
| Charging | On while the pager is on USB power, off the moment it is unplugged |
| Auto | The WiFi radio stays powered down until there is a reason to look: at start-up, when you add a network, and - with GPS on - when you come within about 50 m of the place where a saved network was added. When the network goes out of range the radio powers down again |
| On | Radio stays on and keeps looking |

*Auto* is the one to use on a pager you carry. A network remembers where it was added if the GPS had a position then, or picks one up the next time you are connected with a position; **Saved Networks** marks those *(located)*. Without GPS, Auto only looks at start-up, so switch to *On* when you want it. WiFi being up stops Radio Sleep, and costs battery.

**Check for Update** fetches the release list and shows anything newer than what the pager is running. Turn on **Auto Update Check** and it looks by itself when WiFi connects (once a day at most) and tells you when there is something new. It only tells you; installing is still done the way you installed the first time.

## Web interface

| Meshberry | Mesherola |
|---|---|
| ![The sign-in number, shown when a browser connects, Meshberry](../screenshots/meshberry/web-pin.png) | ![The sign-in number, shown when a browser connects, Mesherola](../screenshots/mesherola/web-pin.png) |
| *The sign-in number, shown when a browser connects* | |

With WiFi connected, the pager serves a page on your local network for messages, contacts, a live map, settings and the SD card's files. Turn it on under *Options → Web Interface*, open the address it shows in a browser on the same network, and type in the six-digit number the pager puts on its screen.

It has a guide of its own, with pictures: **[Web interface](WEB.md)**.

## GPS

*Options → GPS*: **Off**, **On**, or **Power Saver**. Power Saver switches the receiver on just long enough to get a fix, then puts it into standby for ten minutes, so your position can be up to ten minutes old but the receiver uses a small fraction of the power. In standby it keeps what it knows about the satellites, so the next fix is quick. *Share Position* decides whether the mesh is told where you are; it is off unless you turn it on.

## Radio

*Options → LoRa Radio*: region preset, advertise on/off, frequency, bandwidth, spreading factor, coding rate, transmit power, and **Path IDs**. Everyone on a mesh must share frequency, bandwidth and spreading factor.

**Advertise** decides whether the pager announces itself to the mesh at all. **Auto Advert** repeats your advert every 12, 24 or 47 hours. It is off by default and only applies while *Advertise* is on.

Path IDs is 1-byte unless you change it, which every MeshCore node can read. 2-byte and 3-byte make routes more reliable on big meshes, but firmware older than MeshCore 1.14 and some other MeshCore clients cannot read those packets at all: they will not see your messages or your adverts. Only raise it if everything around you is on 1.14 or later.

## Remote admin

| Meshberry | Mesherola |
|---|---|
| ![Logged in to a repeater, Meshberry](../screenshots/meshberry/admin.png) | ![Logged in to a repeater, Mesherola](../screenshots/mesherola/admin.png) |
| *Logged in to a repeater* | |

*Options → Remote Admin* lists the repeaters, room servers and sensors in your contacts. Pick one and enter its password (leave it blank to log in as a guest). Once logged in:

- **Get Status** – battery, uptime, noise floor, last signal, packet counts, air time
- **Get Telemetry** – whatever sensors the node reports
- **Send Command…** – type a console command and read the answer
- **Send Its Advert**, **Sync Its Clock** – the two most common commands, one click each

What you may do depends on the password: guests can read, admins can change things.

## SD card

With a card in at start-up, settings, organizer, ring tones, contacts, channels and messages are kept in a `meshberry` folder on the card. Move the card to another pager running MeshBerry and it starts with all of them. Use a FAT32 card of 32 GB or less.

Your node's private key is **not** on the card. To become the same node on another pager, use *SD Card → Export Private Key…* on the old one and *Import Private Key…* on the new one. Anyone holding a card with an exported key can act as you, so delete `meshberry/private_key.txt` afterwards.

*SD Card* also has: a running **Message Log** (`meshberry/log.txt`, every message as plain text), *Export Messages*, *Eject Card* and *Format Card*.

The *Discovered* list is kept on the card too (`meshberry/heard.bin`), so it is still there after a restart; nodes not heard for 30 days are dropped from it. Without a card the list starts empty each time.

## Phone app

*Options → Bluetooth* turns the companion link on. Pair from the MeshCore app; the default PIN is **012345** and can be changed in the same menu (restart afterwards). Messages you send from the app also appear on the pager.

## Battery life

The biggest savers, in order: GPS off or on *Power Saver*, WiFi off or on *Auto*, a short screen timeout, *Wake Screen* off, Bluetooth off when not using the phone app, the web interface off when nobody is using it.

With the screen off the pager runs slower to save power - except on USB power, or while the web interface is running, where it stays at full speed so that a browser is not kept waiting.

*Options → Device → Power Saver* runs the processor slower. Screens draw a little slower; nothing else changes.

*Options → Device → Radio Sleep (test)* stops the processor while the screen is off and wakes it for incoming packets and key presses. It only takes effect with Bluetooth, GPS and WiFi off and the pager unplugged. It is still being tested and you may miss messages with it on, so the pager asks you to confirm when you switch it on.

---

See also: [Install guide](INSTALL.md) · [FAQ and troubleshooting](FAQ.md) · [MeshBerry Bold 9000](BOLD-9000.md)
