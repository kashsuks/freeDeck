# June 23

Today I had the very bright idea of making my own hackpad from scratch (without the tutorial and no videos etc) in order to get much better at CAD. I realized that my CAD skills are very underwhelming since switching directly from Hackpad v2 to a custom project in which the CAD was pretty complicated. It took me hours on end just to get started and make a very small change.

## Why make a stream deck?

I've gotten quite a bit into streaming programming contests and competitions on my YouTube so I realized that having a stream deck that can help me change scenes, mute/unmute, start/stop stream, etc.

I made my keyboard layout, first I scrolled through the hotkeys section on OBS in order to see which ones I *really* needed, and chose them!

Keyboard Layout:

![Keeb Layout](https://hc-cdn.hel1.your-objectstorage.com/s/v3/5e01f2fea7ed85336f73a7fc70c460d9d3f80123_image.png)

Here is the code for the layout:
```json
["Mute\nUnmute", "Start\nStop", "Countdown"],
["Scene 1", "Scene 2", "Scene 3"],
["Post\nMesg", "Record", "Mute/Un\nScreen"]
```

Total Time Spent This Session: 2 Hours

# June 24

Today I started and *somehow* finished my schematic. I mostly used my experience from me building my hackboard and just recalled and used everything from it. I also made the techincal choice of using a LiPo SHIM in order to simplify the process of charging and having battery protection very simple. For this, I also had to reroute my VCC for the OLED to a GPIO pin and set it to high in order to recieve power.

Here is the picture of my schematic!:

![Schematic](https://hc-cdn.hel1.your-objectstorage.com/s/v3/65dc2a38bf6e3cdce9d213352e33b7ff50abef72_image.png)

The No Connection (NC) pins you see on the first 8 pins on both sides of the Pico are the pins needed for the SHIM. Essentially, you just solder all 16 pins to the SHIM and it *should* work out of the box!

Time Spent This Session: 2 hours
The
