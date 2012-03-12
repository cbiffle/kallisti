Kallisti System Support Package
===============================

This repository records the combinations of software that I use to operate
my MakerBot Cupcake, Kallisti (serial number 69).  I'm recording everything here
for two reasons:

1. I take an "if it ain't broke, don't fix it" approach to operating Kallisti,
   so I change out the software pretty rarely.  This repository helps me
   remember what I'm using before I make changes.
2. I figured this information might help other people who own early-model
   Cupcake printers.

Cloning This Repository
-----------------------

This repository uses git's *submodules* feature to track dependencies.  If you
do a straight-up `git clone` it will leave the submodules empty.  Instead, run

    git clone --recursive


Using This Repository
---------------------

This repository is structured as a set of submodules:

* `ReplicatorG` contains the current preferred version of ReplicatorG from my
  fork.  It has a lot of fixes that haven't yet been merged upstream.
* `G3Firmware-MB` contains the current preferred firmware for the motherboard.
  I build the motherboard and EC from different versions, because my motherboard
  firmware has to be modified to support my 3G5D Shield.
* `G3Firmware-EC` contains the current preferred firmware for the extruder
  controller.  This is mostly a stock version for now.
* `sf_35_profiles` contains my current set of Skeinforge tweaks for my bot.
  These may or may not work for you.  I normally use these together with the
  Print-O-Matic feature in ReplicatorG, which introduces changes that are
  unfortunately difficult to version control.


About Kallisti
--------------

Kallisti is an original-series MakerBot Cupcake printer with a few
modifications.  If you want to use this software to reproduce my results, you'll
want to make sure your 'bot is similar to mine.

* Original Gen3 electronics.
* 3G5D Mini upgrade for stepper extrusion (compatible with the 3G 5D Shield
  available from MakerBot Industries).
* MK6 extruder using 3mm filament --- I've got a lot of filament to use up!
* Heated build platform attached through the extruder controller.

For highest quality, I usually print with PLA plastic, and I always print from
an SD card.
