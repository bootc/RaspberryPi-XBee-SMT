Raspberry Pi XBee ZB SMT Backpack
=================================

This project is for a Raspberry Pi expansion board to accommodate a Digi XBee
ZB SMT board.

The main intention of targeting the ZB SMT is so that the module can be driven
over the SPI bus instead of using the UART. This has several advantages, one of
which is it does not use up the UART so that it can still be used for other
functionality.

The expansion board / backpack is able to host a non-SMT module using the
standard 2mm header. Note that it is impossible to use SPI for modules
connected using this header as the pins are not connected.

Solder jumpers are available to select which SPI chipselect line to use, to
connect the ZB UART to the Raspberry Pi's UART and to connect GPIOs to various
ZB pins (DTR/SLEEP_RQ and INTR).

Submodules
----------

This git repo uses git submodules to pull in SparkFun's Eagle libraries. If you
clone this repo, please run the following commands to pull in the libraries:

```
git submodule init
git submodule update
```

Licensing
---------

<a rel="license" href="http://creativecommons.org/licenses/by-sa/2.0/uk/"><img alt="Creative Commons Licence" style="border-width:0" src="http://i.creativecommons.org/l/by-sa/2.0/uk/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/2.0/uk/">Creative Commons Attribution-ShareAlike 2.0 UK: England &amp; Wales License</a>.

<a target="_blank" href="http://freedomdefined.org/OSHW"><img width="100" alt="OSHW" src="http://summit.oshwa.org/files/2012/04/oshw-logo-100-px.png"></a>

&copy;2012 Chris Boot.

