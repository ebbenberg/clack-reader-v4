# Clack Reader v4
 Esphome component for Clack WS PI (disc valve) Ecosoft LESS and WS1 softener with M5stack TOF sensor saltlevel detection
 
 Relay for control of the chlorinator module from AQMOS
 and Power measurement with ina3221

 Automatic recognision of the softener steps and measure the liters and m3 softened water by reading the clack flowmeter

## 4 Versions / Branches
main: Clack WS PI valve (DiscValve) (ECOSOFT LESS-10 / 15 / 20 from AQMOS)

ws1: Clack WS1 valve (CM(x) from AQMOS)

ws1_usa: Clack WS1 valve with Gallons and Inches / US version

ws1_no_tof: Clack WS1 valve without the TOF sensor code (in case of TOF failure/damaged by water)

Remark: Make sure to copy water_flow.h and tof_vl53l1x.h to your esphome directory before compiling the clack.yaml
There have been some bigger updates to the latest code: added L/min and alarm, also lovelace home assistant menu has been updated.

Remark2: 6 august 2024: Added history regeneration and test button motor pulse to step through regeneration (with time delays stil working between steps)
[example EN](/readme/last_changes_august_2024.jpg)
[example NL](/readme/laaste_wijzigingen_august_2024.jpg)

Remark3: 17 august 2024: Added more options to show the regeneration cycle. Pre fill (dry salt tank) and Post fill (wet salt tank)
Both with or without the 2nd backwash programmed  (between brine and rinse)

      # Pre fill no 2nd Backwash  : FILL/SERVICE/BACKWASH/BRINE/RINSE
      # Pre fill 2nd Backwash     : FILL/SERVICE/BACKWASH/BRINE/BACKWASH2/RINSE
      # Post fill no 2nd Backwash : BACKWASH/BRINE/RINSE/FILL
      # sPost fill 2nd Backwash   : BACKWASH/BRINE/BACKWASH2/RINSE/FILL   

When delivered the Clack reader has already the correct code on the Atom S3 esp.
If needed, there can be downloaded new firmware to the Atom.

***
It is important to connect the TOF sensor to the 4p grove connector near the Atom S3. This needs to be done, before powering the PCB, otherwise the Atom will be in a reboot loop, and no wifi hotspot will be available to connect to.

 ## Dutch:
[README](/readme/clack_uitleg_nl.md)

## English:
[README](/readme/clack_explanation_en.md)

## Contact
Purchase: alphonsuijtdehaag at gmail dot com, if you are interested in a PCB with M5Stack Atom s3 lite

Help: Please open a issue on this git project.

![Example](/readme/pcb_transp.png)



[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/ebbenberg)
