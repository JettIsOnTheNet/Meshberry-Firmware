# FAQ and troubleshooting

**I only see repeaters, no people.**
People appear when they advertise or post. Ask them to send an advert, or check *Address Book → Discovered*.

**Nobody can see me or add me.**
Check *Options → LoRa Radio → Advertise*. It is off unless you answered *On* at first start (it stays off if the set-up was skipped). Turn it on, then send an advert from the Address Book menu.

**My channel message stops short of 160 characters.**
A channel message goes out as "your name: text", and the two together must fit in 160 bytes, so a longer name leaves a little less room. Emoji and accented letters take more than one byte each.

**I can read someone in a channel but cannot message them.**
A private message needs their public key, which arrives with their advert. Use the channel menu → *Message a Person*; the pager will offer to ask them for one.

**My messages get no reply since updating.**
Try *Options → LoRa Radio → Path IDs → 1-byte*. Repeaters on firmware older than MeshCore 1.14 drop 2-byte packets.

**The screen stays off when a message arrives.**
That is the default. Turn on *Options → Alerts → Wake Screen* if you want it lit.

**It will not turn on.**
Hold the wheel for a full second. If the battery was empty, plug in USB.

**The battery percentage looks wrong.**
It is estimated from cell voltage. Tell us the percentage shown and how long it lasted in an issue.

**The map says there is no map data.**
The map needs tiles on the SD card.

**Does it work with the MeshCore phone app?**
Yes, over Bluetooth, as a companion radio. Default PIN 123456. Which is the same combination I have on my luggage.

## Known limits

- LR1121 pagers are not supported yet.
- *Radio Sleep* is a test feature.
- The web interface is plain http, not encrypted. Use it on networks you trust!

## Reporting a problem

Open an issue with: the firmware version (*Options → About*), which style you use, what you did, what you expected and what happened. A photo of the screen helps.
