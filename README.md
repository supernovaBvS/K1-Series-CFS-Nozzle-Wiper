# K1-Series-CFS-Nozzle-Wiper
Creality K1 Series CFS Nozzle Wiper Upgrade 

>This macro replaces the stock Creality Print nozzle wiping routine with a more precise, variable-width scrubbing motion designed specifically for the CFS Purge Chute system.

🛠 Installation
1. SSH into your machine or access via Fluidd/Mainsail
2. Download cfs_nozzle_clear.cfg from this repository and upload to your printer's config directory
3. Add this line to your `printer.cfg` if not already present:
   ```
   [include cfs_nozzle_clear.cfg]
   ```
4. Restart Klipper

⚙️ Configuration
You can customize the wipe behavior directly in the macro or by passing parameters:
- WIPES: Number of back-and-forth passes (Default: 8).
- WIDTH: The total horizontal sweep distance in mm (Default: 13).
- CENTRE_X: If your nozzle isn't hitting the centre of the rubber, adjust this value in the .cfg file (Default: 167.0 for K1C).
- CENTRE_Y: If your nozzle isn't hitting the centre of the rubber, adjust this value in the .cfg file (Default: 226.0 for K1C).

⚠️ Warning for K1 Max Users
The default coordinates in this file are for the K1/K1C. If you are using a K1 Max, you must edit the CENTRE_X and CENTRE_Y coordinates in the .cfg to match your larger build plate's chute position
