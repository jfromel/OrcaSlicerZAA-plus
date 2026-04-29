# OrcaSlicerZAA+

OrcaSlicerZAA+ is a fork of [adob's OrcaSlicer ZAA branch](https://github.com/adob/OrcaSlicer) that adds **extended ironing pattern support**, allowing the ironing pattern to match any of the top surface patterns available in OrcaSlicer.

All Z Contouring (ZAA) work is entirely [@adob's](https://github.com/adob). This fork did not contribute to it in any way.

## What's New in OrcaSlicerZAA+

The only change in this fork is exposing the existing top surface patterns for use with ironing. Previously ironing was limited to Rectilinear and Concentric. OrcaSlicerZAA+ adds all top surface patterns to ironing: Rectilinear, Concentric, Hilbert Curve, Archimedean Chords, Octagram Spiral, Monotonic, Monotonic Line, and Aligned Rectilinear.

## Also Included: Z Contouring (ZAA)

This fork is based on [@adob's](https://github.com/adob) ZAA branch, which implements Z Anti-Aliasing — a non-planar slicing technique that dramatically improves top surface quality. adob's ZAA implementation is currently in review for inclusion in official OrcaSlicer ([PR #12736](https://github.com/OrcaSlicer/OrcaSlicer/pull/12736)).

## Download

Pre-built binaries for Mac, Windows, and Linux are available as artifacts from the latest [GitHub Actions build](https://github.com/jfromel/OrcaSlicerZAA-plus/actions).

## How to Use Extended Ironing Patterns

1. Open **Process settings → Quality tab**
2. Enable **Ironing** and set Ironing type to **All top surfaces**
3. Under **Ironing Pattern**, select any of the 8 available patterns
4. Recommended: Ironing flow 10%, speed 30mm/s, spacing 0.15mm

## How to Use Z Contouring

1. Open **Process settings → Quality tab**
2. Scroll to the **Z Contouring** section
3. Enable **Z contouring enabled**
4. Recommended starting settings: Minimize wall height angle 0°, Minimum z height 0.05mm
5. Slow outer wall and top surface speeds to 20-30mm/s for best results

## Credits

- **Z Anti-Aliasing (Z Contouring)**: [@adob](https://github.com/adob) — [BambuStudio-ZAA](https://github.com
