# Caravel MVP

This is a sample "minimum viable PCB" for [Caravel chips](https://caravel-harness.readthedocs.io/en/latest/): Google MPW or [chipIgnite](https://info.efabless.com/chipignite-v2), including variants for [TinyTapeout](https://tinytapeout.com/).

Fork this repo to get a head start on spinning your own Caravel based PCB.

The circuit includes all the critical (required) elements, basically:

  * power regulation;
  * a clock signal;
  * flash memory, for code; and
  * the chip itself

along with basic passive support (bypass caps...) [Full schematic PDF here](doc/caravel-mvp.pdf)


It also has a few switches and connectors, as demonstrations.  These are enclosed in dotted boxes to highlight their optionality.

![Option Box](https://raw.githubusercontent.com/psychogenic/caravel-mvp/main/doc/img/schem-optionbox.jpg)


The full schematic is available as a PDF in the doc/ directory.

A sample layout was also included, though routing was not completed as you're certainly going to want to change components and floorplan around for your custom boards.


![PCB Floorplan](https://raw.githubusercontent.com/psychogenic/caravel-mvp/main/doc/img/caravel-mvp-floorplan-sample.jpg)


# TinyTapeout

A TinyTapeout-specific versions are also included. The only real differences are in the symbol and net names used, as this helps to clarify things a lot.

If you are implementing a PCB for a TinyTapeout chip, simply:

```
  git checkout tt123
```

and the schematic ([TT version PDF here](doc/caravel-mvp-tinytapeout.pdf)) will include something like this instead:

![TT123 branch](https://raw.githubusercontent.com/psychogenic/caravel-mvp/main/doc/img/tt123-branch.jpg)




# Resources

### TinyTapeout
[TinyTapeout](https://tinytapeout.com/) is an educational project that makes it easier and cheaper than ever to get your digital designs manufactured on a real chip.

It's the easiest and cheapest way I know to get your designs on an ASIC.



### Caravel

Caravel is composed of a harness frame plus two wrappers for drop-in modules for the management area and user project area.  Basically a SoC with a RISC-V CPU, space for user designs and ways to connect those to the outside world.

See:
 * [Caravel chips](https://caravel-harness.readthedocs.io/en/latest/)
 * [efabless/caravel](https://github.com/efabless/caravel)
 * [efabless/caravel_mgmt_soc_litex](https://github.com/efabless/caravel_mgmt_soc_litex)
 







# License

This is meant as a template and starting point for your own projects and is all released under as open hardware.  The MVP schematics and layouts are

  Copyright (C) 2023 Pat Deegan, [Psychogenic Technologies](https://psychogenic.com)

and released under the terms of the Apache License, version 2.0.  See the accompanying LICENSE file for details.

