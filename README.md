# IMPOSE — Serum 2 Bass Pack

24 analog / tech-house / reese / acid / 808 / growl bass patches as **real Serum 1 `.fxp` files**.

Cloned from the attached Serum 1 preset `AU_MT_bass_memories_imposing` (Organics / AC hum1). Oscillator, filter, envelope, LFO and FX knobs are morphed per patch. Wavetable + hum sample stay from the original so Serum will load them.

Serum 2 opens Serum 1 `.fxp` on drag-and-drop.

## Download

- **[IMPOSE_Serum2_Bass_Pack.zip](https://github.com/djOffstage/impose-serum-bass-pack/raw/main/IMPOSE_Serum2_Bass_Pack.zip)**
- **[24 .fxp files](https://github.com/djOffstage/impose-serum-bass-pack/tree/main/FXP)**
- **[Original reference .fxp](https://github.com/djOffstage/impose-serum-bass-pack/raw/main/Original/AU_MTF_bass_synth_memories_imposing.fxp)**

## Install

1. Drag any `FXP/*.fxp` onto Serum 2.
2. Or copy into `Documents/Xfer/Serum 2 Presets/User/IMPOSE/` and **Rescan folders on disk**.

## How the .fxp files were made

Serum 1 `.fxp` = VST2 header (`CcnK` / `FPCh` / `XfsX`) + zlib chunk. ~300 little-endian floats at offset `0x3460` follow Xfer `SYParameters.txt` order. Each IMPOSE patch starts from the decompressed original, writes those floats, updates the name, recompresses.

Unsigned `.SerumPreset` (Serum 2 CBOR) files are not generated — those crash when invented from scratch.
