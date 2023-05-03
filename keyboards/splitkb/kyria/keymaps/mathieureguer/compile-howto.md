# Compiling QMK keymap

move to your custom keymap directory:

```
cd /Users/mathieu/qmk_firmware/keyboards/splitkb/kyria/keymaps/mathieureguer
```

compile the keymap, with a converter for the controler

```
qmk compile -e CONVERT_TO=elite_pi
```

reset the keyboard and copy the .uf2 file to the keyboard drive.
There is a mac bug preventing drag and drop copying. Use terminal cp instead.

```
cp /Users/mathieu/qmk_firmware/splitkb_kyria_rev3_mathieureguer_elite_pi.uf2 /Volumes/RPI-RP2/splitkb_kyria_rev3_mathieureguer_elite_pi.uf2
```