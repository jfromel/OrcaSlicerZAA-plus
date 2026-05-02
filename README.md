# OrcaSlicerZAA+

OrcaSlicerZAA+ is a fork of [adob's OrcaSlicer ZAA branch](https://github.com/adob/OrcaSlicer) that adds **bottom layer ZAA, support ZAA and extented ironing patterns**, allowing the ironing pattern to match any of the top surface patterns available in OrcaSlicer. It also includes tool tips for the ZAA to full wiki at https://github.com/jfromel/OrcaSlicerZAA-plus/wiki

All Z Contouring (ZAA) top surface work is entirely [@adob's](https://github.com/adob), et al. Contributions from this fork include bottom surface ZAA, UI improvements, tool tips, wiki, and recommended default values.

## What's New in OrcaSlicerZAA+

This fork exposes the existing top surface patterns for use with ironing. Previously ironing was limited to Rectilinear and Concentric. OrcaSlicerZAA+ adds all top surface patterns to ironing: Rectilinear, Concentric, Hilbert Curve, Archimedean Chords, Octagram Spiral, Monotonic, Monotonic Line, and Aligned Rectilinear.

## Also Included: Z Contouring (ZAA)

This fork is based on [@adob's](https://github.com/adob) ZAA branch, which implements Z Anti-Aliasing — a non-planar slicing technique that dramatically improves top surface quality. adob's ZAA implementation is currently in review for inclusion in official OrcaSlicer ([PR #12736](https://github.com/OrcaSlicer/OrcaSlicer/pull/12736)). This version also includes ZAA for bottom layers and support interface layers. 

## Download

Pre-built binaries for Mac, Windows, and Linux are available as artifacts from the latest [GitHub Actions build](https://github.com/jfromel/OrcaSlicerZAA-plus/actions).

## How to Use Extended Ironing Patterns

1. Open **Process settings -> Quality tab**
2. Enable **Ironing** and set Ironing type to **All top surfaces**
3. Under **Ironing Pattern**, select any of the 8 available patterns
4. Recommended: Ironing flow 10%, speed 30mm/s, spacing 0.15mm

## How to Use Z Contouring

1. Open **Process settings -> Quality tab**
2. Scroll to the **Z Contouring** section
3. Enable **Z Contour Top** for top surface contouring
4. Recommended starting settings: Minimum z height 0.02mm, Minimize wall height angle 35°
5. Enable **Z Contour Bottom** for bottom surface contouring (requires support material)
6. Slow outer wall and top surface speeds to 20-30mm/s for best results

## Credits

- **Z Anti-Aliasing (Z Contouring)**: [@adob](https://github.com/adob) — [BambuStudio-ZAA](https://github.com/adob/BambuStudio-ZAA) and [OrcaSlicer PR #12736](https://github.com/OrcaSlicer/OrcaSlicer/pull/12736). All ZAA/Z Contouring work is adob's — this fork refines the UI pending PR.
- **Original ZAA post-processing script**: [@Theaninova](https://github.com/Theaninova) — [GCodeZAA](https://github.com/Theaninova/GCodeZAA)
- **ZAA research**: [Anti-aliasing for fused filament deposition](https://arxiv.org/abs/1609.03032) by Hai-Chuan Song et al.
- **OrcaSlicer**: [@SoftFever](https://github.com/SoftFever) and the OrcaSlicer community
- **Extended ironing patterns**: [@jfromel](https://github.com/jfromel) — Exposed existing top surface patterns for use with ironing, so the ironing pattern can match the top surface pattern.
- **Bottom surface ZAA**: [@jfromel](https://github.com/jfromel) — Z Contouring for bottom surfaces with support interface contouring, per-object disable, and UI reorganization (Top/Bottom sections with toggle controls).

## Contributing

OrcaSlicerZAA+ is maintained by a manufacturer who utilizes FDM printing. I am not a professional developer, I just wanted a slicer that did a bit more than what's currently available. Pull requests won't be actively reviewed or merged here — but you're welcome to fork this repo and take it wherever you want! If the extended ZAA features and ironing patterns are useful, consider submitting them upstream to [OrcaSlicer](https://github.com/OrcaSlicer/OrcaSlicer/pulls). For Z Contouring improvements, contribute directly to [@adob's PR](https://github.com/OrcaSlicer/OrcaSlicer/pull/12736).

## Support This Project

If OrcaSlicerZAA+ has improved your prints, a small donation is always appreciated!

[![Donate via PayPal](https://img.shields.io/badge/Donate-PayPal-blue.svg)](https://paypal.me/jfromel)

## License

OrcaSlicerZAA+ is licensed under the **GNU Affero General Public License v3.0**, the same license as OrcaSlicer.
