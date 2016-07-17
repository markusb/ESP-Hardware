<H1>ESP-Hardware</H1>
<p>This repository contains my collection of ESP-Related hardware designs

<h2>ESP-8285 Miniboard</h2>

<p>Small DIL-size board for an ESP8285 Wifi microcontroller
<p>There already are a bunch of ESP boards and modules around, but the either add a full programming circuit or are modules with small pins to solder.
<p>This wants to combine the best of both, with standard 2.54mm pinheaders and easy programming, but on a separate board. So you plug in the programmer when you want to download firmware, but remove it when you don't need it anymore.
<ul>
<li>DIL size, plugs directly into a breadboard
<li>Breaks out all IO pins, not an arbitrary selection like most modules
<li>Antenna and crystal on board, ready to, just add power
<li>Optional red power and blue tx LED, to see whats going on, can be removed to save power
<li>No other, potentially unwanted hardware to get in the way of your design
</ul>

<h2>ESP82xx Programmer</H2>
<p>USB programmer built for the ESP-Miniboard, but it will work for normal ESP82xx circuits and most modules as well.
<p>As the ESP-Miniboard has no programmer, you need it separately. So it goes on this second board, to be removed when no longer in use.
<ul>
<li>USB-Serial chip (CH340)
<li>3.3V Regulator to feed the ESP from USB during programming (no external power needed)
<li>3.3V supply has a jumper to disable power and a polyfuse to protect from a short
<li>Nodemcu reset circuit to decouple the RTS/DTR lines from reset and GPIO0
<li>Works with any ESP module, just connect up the pins and off you go !
</ul>
