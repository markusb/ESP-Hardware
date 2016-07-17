# ESP-Hardware


<h1>ESP-8285 Miniboard</h1>

<p>Small DIL-size board for an ESP8285 Wifi microcontroller
<ul>
<li>DIL size
<li>Breaks out all IO pins
<li>Antenna and crystal on board
<li>Optional rep power and blue tx LED
<li>No potentially unwanted hardware
</ul>
<h1>ESP82xx Programmer</H1>
<p>USB programmer built for the ESP-Miniboard, but it will work for normal ESP82xx circuits and most modules as well.
<ul>
<li>USB-Serial chip (CH340)
<li>3.3V Regulator to feed the ESP from USB during programming (no external power needed)
<li>3.3V supply has a jumper to disable power and a polyfuse to protect from a short
<li>Nodemcu reset circuit to decouple the RTS/DTR lines from reset and GPIO0
</ul>
