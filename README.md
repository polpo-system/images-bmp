# images-bmp

BMPImages for [polpo](https://github.com/polpo-system/polpo): the reader of Windows bitmaps (.bmp) for the Images package of ETH Oberon (the
package images). With it, Images.Load reads .bmp files (`bmp = BMPImages.Install` in the section
ImageFormats of Oberon.Text), so every program on Images shows them.

```
portia.Install images-bmp
```

## What is here

    src/BMPImages.Mod
    test/BMPImagesTest.Mod

The source comes from ETH Linux Oberon (OLR, 2017-06-18), converted from an Oberon text to plain
text; the first commit has it unchanged. It compiles unchanged with all five of polpo's compilers
(x86, ARM, ARMv7, RISC-V, MIPS). It reads bitmaps of 1 to 32 bits; it does not write them.

## Tests

    BMPImagesTest.Run      2 checks: a 2 by 1 bitmap written and loaded; it needs the desktop's
                           display

The license is GPL-3 (`LICENSE`); the code comes from ETH Oberon, whose license (`LICENSE.ETH`)
asks to keep its copyright notice and conditions, which `LICENSE.ETH` does.
