# retroflag-picase
## RetroFlag Pi-Case+ Safe Shutdown

#### Turn switch "SAFE SHUTDOWN" on PCB to ON position.

![Safe Shutdown Switch](http://retroflag.com/images/nespi_case+/safe_shutdown.jpg "Safe Shutdown Switch")

This is a fork of [esisco](https://github.com/esisco)'s fork that translated the basic outline of [crcerror](https://github.com/crcerror)'s [multi_switch.sh](https://github.com/crcerror/retroflag-picase/blob/master/multi_switch.sh) Bash script into Python and neatly packed into the existing [SafeShutdown.py](../SafeShutdown.py) Python script. The thing shuts the Pi down more properly than the original script and saves metadata with it. This fork just modifies the script a bit to act more like the NES Classic Edition. It also fixes some things that didn't make sense.

Changes:
- Pressing "RESET" will ONLY exit a game, if not in ES, it will clear the terminal.

--------------------
**_ONLY FOR RETROPIE!_**   (I might try to do it for RecalBox if I have time.)
--------------------

Example for RetroPie:
1. Make sure internet is connected.
2. Make sure keyboard is connected.
3. Press F4 to enter terminal.
4. In the terminal, type the one-line command below(Case sensitive):

```bash
wget -O - "https://raw.githubusercontent.com/PokeEngineer/retroflag-picase/master/install.sh" | sudo bash
```

--------------------

Example for RecalBox:
1. Make sure internet is connected.
2. Make sure keyboard is connected.
3. Press F4 first. Then press ALT-F2 to enter terminal.
4. User:root Password:recalboxroot
5. In the terminal, type the one-line command below(Case sensitive):

```bash
wget -O - "https://raw.githubusercontent.com/RetroFlag/retroflag-picase/master/recalbox_install.sh" | bash
```
