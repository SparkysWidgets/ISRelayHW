Welcome To: ISRelay Hardware Repo!!
================================

##### Note: This is for the In Series Relay Hardware Version .13 Branch

ISRelay Hardware Design Files in EAGLE. Not much to say, Is consists of mainly Stock parts and is a PTH version!

Schematic Info
-------------------------
##### Schematic is basic and fairly self explanatory

- Input header/Connector (This is usually from a 5V low power MCU)
- BJT acting as a DC current gain switch(~5mA through the BE junction)
- Relay for circuit Isolation from mains
- Flyback, reverse voltage spike protection diode
- LOAD header for connection in series with the HOT line of the mains wiring to be switch
- Added frame to better capture version and project info and license for both board and schem
- Brought info in frame up to date to new site URL schema

Board Layout Info
-------------------------
##### Form Factor based on minimum footprint that can fit this sized relay, can fit into deep outlet boxes

- Creep-age distance between HOT and LV digital side was increased significantly over v11
- Internal cutout added to help the Isolation ^
- Large enough traces to match Relay load specs
- Added traces for LOAD on both sides of PCB as recommended by Relay MFG
- Lengthened traces to both contact sets as recommended by Relay MFG
- Lower portion of GND plane moved!
- Upper portion of GND plane moved!
- Added a bit of a hook up legend below LV connector
- increased creep-age cutout slightly
- changed silk info to reflect new site URL schema

Errata
-------------------------

##### Just a quick list of current issues
- Silkscreen improvements as always 
- Tweak traces a tad bit

Firmware
-------------------------

- There is no firmware (YEEEEES) Feed the control anywhere from ~3.3v to 5v, 5v(higher current source ~80mA for the RZSchrack, and ~100mA for the TE relay)

Using an Arduino to switch on a lamp (DIY Powerswitch tail has never been better!)
-------------------------

A while ago when I first when on this Garden automation adventure(around 2005-06ish), I came across a problem of needed to switch mains pumps, fans and lights. This was before the PST and Sparkfuns Big boy relay kits existed, so I went about source a great relay and some parts to bring it all together.
Since then my awesome much loved Relay is no longer readily available and the similar replacements while adequate don't work quite as well (not a big deal some of the other features are better!)

Feed it 5v, Gnd and a small current ~5ma 5V control signal and the relay does the rest. The units are designed to switch the HOT portion of mains just like a light switch, and use a relay with a high enough specs to drive inductive loads in the range of about 10amps.


Please see [ISRelay's project page](http://www.sparkyswidgets.com/portfolio-item/relaypcb/) for more information!
<http://www.sparkyswidgets.com/portfolio-item/relaypcb/>


License Info
-------------------------

<a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/deed.en_US"><img alt="Creative Commons License" style="border-width: 0px;" src="http://i.creativecommons.org/l/by-sa/3.0/88x31.png" /></a><br />
<span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">ISRelay</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="www.sparkyswidgets.com" property="cc:attributionName" rel="cc:attributionURL">Ryan Edwards, Sparky's Widgets</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/deed.en_US">Creative Commons Attribution-ShareAlike 3.0 Unported License</a>.<br />
Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="http://www.sparkyswidgets.com/portfolio-item/relaypcb/" rel="dct:source">http://www.sparkyswidgets.com/portfolio-item/relaypcb/</a>