# Smart Ropewalk v3.68

## What's new

- Preset names now include the final diameter and RH/LH direction; custom titles are preserved.
- The recipe editor shows RH/LH and a trash button with deletion confirmation. Deleted slots stay empty after restart and can be reused.
- The preset list has more room for names: motor RPM are no longer shown; twist/winding targets and final diameter remain visible.
- Apply saves the recipe and returns to the main working page without starting motors. Save returns to the list. A writable SD card is required for saving.
- Opening a preset preserves its saved final diameter.
- Web Display shows Display busy during temporary screen delays and resumes automatically. Touch commands are never retried automatically.
- Updated Italian, English and Spanish PDF manuals with current screenshots and callouts; updated optional Web Display ZIP.

Motor settings, calculation formulas, activation, rigging database rev70 and ship images rev69 are unchanged. Existing saved recipes are preserved during the update.

## Data update 2026-10-31

Rigging database **rev71** and ship images **rev70** are now available separately, with the same firmware 3.68 binary. Use **UPDATE DATA**, not firmware installation. The package includes 333 kits and 13,421 rigging rows, a dedicated Amerigo Vespucci table (249 entries marked as modelling estimates), seven Vespucci kit/scale variants, and Redoutable by Artesania Latina at 1:84 with its background image.

Existing Steel data are unchanged. Missing diameters remain n.d.; Vespucci directions assigned by analogy are documented in the CSV notes. See [database rev71 notes](../rigging-rev71/README.md) and the optional [data ZIP](../rigging-rev71/Smart-Ropewalk-Rigging-rev71.zip). No particular firmware/data update order is required.

## Web Display

Connect the machine and your computer or tablet to the same local network, read the machine IP on its Wi-Fi page, then open `http://` followed by that IP in your browser. Reload the page after updating firmware.

Alternatively, extract the complete optional ZIP on a computer, open index.html, enter the machine IP and select Connect. The ZIP includes instructions in all three languages.

Tested with Edge on Windows and WebKit using iPad profiles. iPadOS 15 or later is the target requirement; a physical iPad and macOS Safari have not been tested.

**Safety:** this panel controls the real machine. Closing the browser or losing Wi-Fi does not stop motors. Demo-mode restrictions remain active.

## Update and manuals

For OTA use the application `.bin`, not the merged image. The merged image is for complete USB installation and can overwrite internal settings.

The updated PDF manuals are downloaded automatically during firmware OTA when newer or missing. They are also available individually below. No separate database update is required for this firmware release.
