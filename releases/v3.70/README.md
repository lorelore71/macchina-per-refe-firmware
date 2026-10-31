# Smart Ropewalk 3.70

## What changed

- In Rope calculation, the input field is now named Requested diameter (Italian: Diametro richiesto; Spanish: Diametro solicitado). This distinguishes the requested input from the Obtainable result below it.
- This is a wording change only. Calculation formulas, motor control, pin mapping, saved recipes, Wi-Fi settings and activation are unchanged.
- Updated Italian, English and Spanish PDF manuals and the optional Web Display ZIP. The Web Display mirrors the new label automatically after updating the firmware and reloading the page.
- Rigging database rev71 and ship images rev70 are unchanged. The ongoing catalogue review is not part of this release.

## Update

Manual refresh, 1 November 2026: the three PDF manuals now include native
3.70 display screenshots and matching calculation callouts, including the
repeated screen in the working procedure. Firmware binaries, Web Display
ZIP and rigging data are unchanged. The OTA manual package date was advanced.

Use the application `.bin` for OTA, not the merged image. The merged image is for full USB installation and can overwrite internal settings.

The PDF manuals are downloaded automatically during firmware OTA when newer or missing. Saved recipes are preserved. No database update is required for this firmware change.

Open `http://` followed by the display IP on the same Wi-Fi network. The optional ZIP includes instructions in English, Italian and Spanish.

Safety: this interface controls the real machine. Closing the browser or losing Wi-Fi does not stop motors. Demo-mode restrictions remain active.
