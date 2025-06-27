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

**Total Time Spent This Session**: 2 Hours

# June 24

Today I started and *somehow* finished my schematic. I mostly used my experience from me building my hackboard and just recalled and used everything from it. I also made the techincal choice of using a LiPo SHIM in order to simplify the process of charging and having battery protection very simple. For this, I also had to reroute my VCC for the OLED to a GPIO pin and set it to high in order to recieve power.

Here is the picture of my schematic!:

![Schematic](https://hc-cdn.hel1.your-objectstorage.com/s/v3/65dc2a38bf6e3cdce9d213352e33b7ff50abef72_image.png)

The No Connection (NC) pins you see on the first 8 pins on both sides of the Pico are the pins needed for the SHIM. Essentially, you just solder all 16 pins to the SHIM and it *should* work out of the box!

I also got started on my PCB and encountered a very big problem, the LiPo batteries online are too big for my current size. Once a PCB exceeds 100x100mm, its price can increase significantly. The average 100MaH LiPo battery is approx 20x40mm which means it takes up a big chunk of my size, other than that most things are going pretty well.

I did have to research the spacing for cherry mx switches in order to have proper spacing. Unlike the choc which had gap in between each switch, the cherry mx switches sit beside each other, which I think is amazing for compact designs like a macropad!

Here is what I have for my PCB so far:

![Unfinished PCB](https://hc-cdn.hel1.your-objectstorage.com/s/v3/660447d9d6ce91159810b8ea82c55892988ea420_image.png)

**Time Spent This Session**: 3 hours


# June 27

This day was uhh pretty tough. First, I realized that my lipi battery would not fit if I were to use a pico. Thats when someone told me about the XIAO RP2040ESPC3 which has battery management inbuilt that uses a B+ and  B- pin. That means that if I use a lipo without a JST connector, I can just solder the red to +ve and black to -ve and it _should__ work out of the box.

So I got to work, first I updated my schematic to use the C3's symbol (DIP). This didnt take long since it was just changing the wires. 

![Update Schematic](https://hc-cdn.hel1.your-objectstorage.com/s/v3/6554559b3b1b1dc44942cf5ad7a5e87cb2cde7de_image.png)

And....

I also worked on the pcb!!

This was a bit more difficult since I had to delete all my progress so far and just restart with the new components. This change also allowed me possibly add a larger lipo battery.

And heres what I have so far for my PCB:

![Updated PCB](https://hc-cdn.hel1.your-objectstorage.com/s/v3/678cc5a84d751f1c1bee1c185a9f40fd0722f42e_image.png)

**Total Time Spent This Session**: 2 Hours
