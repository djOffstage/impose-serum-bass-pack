IMPOSE — Serum 2 Bass Pack
24 analog / tech-house / reese / acid / 808 / growl patches
Inspired by AU_MT_bass_memories_imposing (Organics / AC hum1)

============================================================
WHAT IS IN THIS ZIP
============================================================
/FXP/        24 Serum 1 .fxp patches — drag onto Serum 2
/Original/   The reference Memories Imposing .fxp you supplied
/Recipes/    Text sheets (wavetables, macros, matrix)
/JSON/       Machine-readable recipes

============================================================
SERUM 2 — HOW TO INSTALL THE .FXP FILES
============================================================
1. Drag any file in /FXP/ onto Serum 2, or:
     Menu → Open Preset → pick the .fxp
   Serum 2 converts Serum 1 .fxp on load.

2. To keep them in the browser:
     Documents/Xfer/Serum 2 Presets/User/IMPOSE/
   then Menu → Rescan folders on disk.

The 24 .fxp files are clones of YOUR Memories Imposing preset
with oscillator, filter, envelope, LFO, FX and on/off knobs
morphed per patch. Wavetable data and the Organics/AC hum1
noise sample stay from the original so the files stay valid.

============================================================
HOW THESE .FXP FILES WERE MADE
============================================================
Serum 1 .fxp = VST2 header (CcnK/FPCh/XfsX) + zlib chunk.
Inside the decompressed chunk, ~300 little-endian floats at
offset 0x3460 follow Xfer's SYParameters.txt order
(MasterVol, A Vol, A Octave, Filter Cutoff, Env1, Dist, …).

Each IMPOSE patch starts from the decompressed original,
writes those floats, updates the preset name, then
recompresses. Unsigned .SerumPreset (Serum 2 CBOR) files
are still not generated — those crash when invented from
scratch. Serum 1 .fxp is the format your reference used,
and Serum 2 loads it.

============================================================
PLAYING NOTES
============================================================
Range     C1–C3 (sub lives at C1; C2 reads on laptop speakers)
Mono      recommended on HUM / SUB / 808
Wobbles   hold a note, lock LFO to host
Macros    1 Drive   2 Width   3 Dark   4 Texture / Hum

Pack  IMPOSE 1.1
