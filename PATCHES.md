# Select Your Version

 * [American Release, revision 0](#american-release-revision-0)
 * [American Release, revision 1](#american-release-revision-1)
 * [American Release, unknown revision](#american-release-unknown-revision)
 * [Japanese Release, revision 0](#japanese-release-revision-0)
 * [Japanese Release, revision 1](#japanese-release-revision-1)
 * [Japanese Release, unknown revision](#japanese-release-unknown-revision)
 * [European Release](#european-release)
 * [Korean Release](#korean-release)
 * [Unknown Version (How to identify your copy's version)](#unknown-version)

## American Release, revision 0

IPS Patch: [S.MARIO64DS_ASME01_00.ips](//raw.githubusercontent.com/LRFLEW/AM64DS_DeSmuME/analog/patches/S.MARIO64DS_ASME01_00.ips)

Cheat Code:
```
020244EC EA00000C
E202B320 00000040
E3A03301 E3833F81
E1D300B0 E3C00080
E1C300B0 E3A03409
E3833C01 E8930003
E3700001 03A00000
03A01000 E2893008
E8830003 E3A00001
E5C90014 EA0000B4
E2073324 00000008
02000100 00000000
520F0D88 E7D22001
020F0D88 E3A02000
D0000000 00000000
520F2584 E19100B0
020F2584 EA000070
D2000000 00000000
```

## American Release, revision 1

IPS Patch: [S.MARIO64DS_ASME01_01.ips](//raw.githubusercontent.com/LRFLEW/AM64DS_DeSmuME/analog/patches/S.MARIO64DS_ASME01_01.ips)

Cheat Code:
```
02024760 EA00000C
E202B5E4 00000040
E3A03301 E3833F81
E1D300B0 E3C00080
E1C300B0 E3A03409
E3833C01 E8930003
E3700001 03A00000
03A01000 E2893008
E8830003 E3A00001
E5C90014 EA0000B4
E2074044 00000008
02000100 00000000
520F2848 E7D22001
020F2848 E3A02000
D0000000 00000000
520F4058 E19100B0
020F4058 EA000070
D2000000 00000000
```

## American Release, unknown revision

You can identify the revision of a game cartridge by the black text printed on the back. If it is `ASMEN0J20`, then it's [revision 0](#american-release-revision-0), and if it's `ASMEN1J12` or `ASMEN1J22`, then it's [revision 1](#american-release-revision-1).

You can identify the revision of a ROM file with a hex editor. The byte at address `0x1E` is `00` for [revision 0](#american-release-revision-0) and `01` for [revision 1](#american-release-revision-1).

If you still are unsure, you can use the following cheat code, which will detect your game revision and apply the right patch:

```
823FFE1E 00000000
D3000000 00000274
D0000000 00000000
020244EC EA00000C
823FFE1E 00000000
D3000000 000002C4
D0000000 00000000
E202B320 00000040
E3A03301 E3833F81
E1D300B0 E3C00080
E1C300B0 E3A03409
E3833C01 E8930003
E3700001 03A00000
03A01000 E2893008
E8830003 E3A00001
E5C90014 EA0000B4
823FFE1E 00000000
D3000000 00000D20
D0000000 00000000
E2073324 00000008
02000100 00000000
D3000000 020F0D88
823FFE1E 00000000
DC000000 00001AC0
D0000000 00000000
50000000 E7D22001
00000000 E3A02000
D0000000 00000000
D3000000 020F2584
823FFE1E 00000000
DC000000 00001AD4
D0000000 00000000
50000000 E19100B0
00000000 EA000070
D2000000 00000000
```

## Japanese Release, revision 0

IPS Patch: [S.MARIO64DS_ASMJ01_00.ips](//raw.githubusercontent.com/LRFLEW/AM64DS_DeSmuME/analog/patches/S.MARIO64DS_ASMJ01_00.ips)

Cheat Code:
```
02024724 EA00000C
E202B5A8 00000040
E3A03301 E3833F81
E1D300B0 E3C00080
E1C300B0 E3A03409
E3833C01 E8930003
E3700001 03A00000
03A01000 E2893008
E8830003 E3A00001
E5C90014 EA0000B4
E20738C8 00000008
02000100 00000000
520F0588 E7D22001
020F0588 E3A02000
D0000000 00000000
520F1D98 E19100B0
020F1D98 EA000070
D2000000 00000000
```

## Japanese Release, revision 1

IPS Patch: [S.MARIO64DS_ASMJ01_01.ips](//raw.githubusercontent.com/LRFLEW/AM64DS_DeSmuME/analog/patches/S.MARIO64DS_ASMJ01_01.ips)

Cheat Code:
```
0202475C EA00000C
E202B5E0 00000040
E3A03301 E3833F81
E1D300B0 E3C00080
E1C300B0 E3A03409
E3833C01 E8930003
E3700001 03A00000
03A01000 E2893008
E8830003 E3A00001
E5C90014 EA0000B4
E2074168 00000008
02000100 00000000
520F1768 E7D22001
020F1768 E3A02000
D0000000 00000000
520F2F78 E19100B0
020F2F78 EA000070
D2000000 00000000
```

## Japanese Release, unknown revision

You should be able to identify a revision of the game cartridge by the black text printed on the back. I couldn't find any information online about the Japanese version, but it seems likely that if it is `ASMJN0J**`, then it's [revision 0](#japanese-release-revision-0), and if it's `ASMJN1J**`, then it's [revision 1](#japanese-release-revision-0) (with `*` being any numeric digit).

You can identify the revision of a ROM file with a hex editor. The byte at address `0x1E` is `00` for [revision 0](#japanese-release-revision-0) and `01` for [revision 1](#japanese-release-revision-1).

If you still are unsure, you can use the following cheat code, which will detect your game revision and apply the right patch:

```
823FFE1E 00000000
D3000000 00000038
D0000000 00000000
02024724 EA00000C
823FFE1E 00000000
D3000000 00000038
D0000000 00000000
E202B5A8 00000040
E3A03301 E3833F81
E1D300B0 E3C00080
E1C300B0 E3A03409
E3833C01 E8930003
E3700001 03A00000
03A01000 E2893008
E8830003 E3A00001
E5C90014 EA0000B4
823FFE1E 00000000
D3000000 000008A0
D0000000 00000000
E20738C8 00000008
02000100 00000000
D3000000 020F0588
823FFE1E 00000000
DC000000 000011E0
D0000000 00000000
50000000 E7D22001
00000000 E3A02000
D0000000 00000000
D3000000 020F1D98
823FFE1E 00000000
DC000000 000011E0
D0000000 00000000
50000000 E19100B0
00000000 EA000070
D2000000 00000000
```

## European Release

IPS Patch: [S.MARIO64DS_ASMP01_00.ips](//raw.githubusercontent.com/LRFLEW/AM64DS_DeSmuME/analog/patches/S.MARIO64DS_ASMP01_00.ips)

Cheat Code:
```
02024D60 EA00000C
E202C404 00000040
E3A03301 E3833F81
E1D300B0 E3C00080
E1C300B0 E3A03409
E3833C01 E8930003
E3700001 03A00000
03A01000 E2893008
E8830003 E3A00001
E5C90014 EA0000B4
E2075658 00000008
02000100 00000000
520FA7C0 E7D22001
020FA7C0 E3A02000
D0000000 00000000
520FC0C0 E19100B0
020FC0C0 EA000070
D2000000 00000000
```

## Korean Release

IPS Patch: [S.MARIO64DS_ASMK01_00.ips](//raw.githubusercontent.com/LRFLEW/AM64DS_DeSmuME/analog/patches/S.MARIO64DS_ASMK01_00.ips)

Cheat Code:
```
02024A68 EA00000C
E202B3E4 00000040
E3A03301 E3833F81
E1D300B0 E3C00080
E1C300B0 E3A03409
E3833C01 E8930003
E3700001 03A00000
03A01000 E2893008
E8830003 E3A00001
E5C90014 EA0000B4
E206FF14 00000008
02000100 00000000
520F9780 E7D22001
020F9780 E3A02000
D0000000 00000000
520FAFB4 E19100B0
020FAFB4 EA000070
D2000000 00000000
```

## Unknown Version

You can identify the region of a game cartridge by the text at the bottom of the front of the cartridge. There will be a product code of the form `NTR-XXXX-XXX`. The middle 4 letters identify the version of the game. `ASME` means [American](#american-release-unknown-revision), `ASMJ` means [Japanese](#japanese-release-unknown-revision), `ASMP` means [European](#european-release), and `ASMK` means [Korean](#korean-release).

You can identify the region of a ROM file with a hex editor. The four bytes starting at `0x0C` are the ascii characters of the four letter codes on the game cartridge. Find the code from the list in the previous paragraph to identify the version.

You can also identify the game version by version differences. The [Japanese version](#japanese-release-unknown-revision) has a blue Nintendo logo at the start and is in Japanese. The [Korean version](#korean-release) has a black Nintendo logo at the start, is in Korean, and does not have a button on the main menu for the minigames. Both the American and European releases have a red Nintendo logo at the start, but the [European version](#european-release) matches the console's language (English, French, German, Spanish, and Italian), while the [American version](#american-release-unknown-revision) is always in English.

If you cannot figure out which version you have, you can use the following cheat code, which will detect your game version and apply the right patch. It is **recommended** that you use a version-specific patch, as this code is significantly more version detection than patching, but it *is* an option if you need it. Note: this code still only works with the versions with version-specific codes, and won't work with other versions, such as Demo builds.

```
523FFE0C 454D5341
D3000000 02024760
923FFE1E 00000000
D3000000 020244EC
D0000000 00000000
D0000000 00000000
523FFE0C 4A4D5341
D3000000 0202475C
923FFE1E 00000000
D3000000 02024724
D0000000 00000000
D0000000 00000000
523FFE0C 504D5341
D3000000 02024D60
D0000000 00000000
523FFE0C 4B4D5341
D3000000 02024A68
D0000000 00000000
00000000 EA00000C
523FFE0C 454D5341
D3000000 0202B5E4
923FFE1E 00000000
D3000000 0202B320
D0000000 00000000
D0000000 00000000
523FFE0C 4A4D5341
D3000000 0202B5E0
923FFE1E 00000000
D3000000 0202B5A8
D0000000 00000000
D0000000 00000000
523FFE0C 504D5341
D3000000 0202C404
D0000000 00000000
523FFE0C 4B4D5341
D3000000 0202B3E4
D0000000 00000000
E0000000 00000040
E3A03301 E3833F81
E1D300B0 E3C00080
E1C300B0 E3A03409
E3833C01 E8930003
E3700001 03A00000
03A01000 E2893008
E8830003 E3A00001
E5C90014 EA0000B4
523FFE0C 454D5341
D3000000 02074044
923FFE1E 00000000
D3000000 02073324
D0000000 00000000
D0000000 00000000
523FFE0C 4A4D5341
D3000000 02074168
923FFE1E 00000000
D3000000 020738C8
D0000000 00000000
D0000000 00000000
523FFE0C 504D5341
D3000000 02075658
D0000000 00000000
523FFE0C 4B4D5341
D3000000 0206FF14
D0000000 00000000
E0000000 00000008
02000100 00000000
523FFE0C 454D5341
D3000000 020F2848
923FFE1E 00000000
D3000000 020F0D88
D0000000 00000000
D0000000 00000000
523FFE0C 4A4D5341
D3000000 020F1768
923FFE1E 00000000
D3000000 020F0588
D0000000 00000000
D0000000 00000000
523FFE0C 504D5341
D3000000 020FA7C0
D0000000 00000000
523FFE0C 4B4D5341
D3000000 020F9780
D0000000 00000000
50000000 E7D22001
00000000 E3A02000
D2000000 00000000
523FFE0C 454D5341
D3000000 020F4058
923FFE1E 00000000
D3000000 020F2584
D0000000 00000000
D0000000 00000000
523FFE0C 4A4D5341
D3000000 020F2F78
923FFE1E 00000000
D3000000 020F1D98
D0000000 00000000
D0000000 00000000
523FFE0C 504D5341
D3000000 020FC0C0
D0000000 00000000
523FFE0C 4B4D5341
D3000000 020FAFB4
D0000000 00000000
50000000 E19100B0
00000000 EA000070
D2000000 00000000
```