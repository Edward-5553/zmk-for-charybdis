# Charybdis 4x6 ZMK configuration

This configuration targets a 58-key split Charybdis with five thumb keys on
each side and no trackball. The right half remains the central half.

The two added right thumb switches reuse the existing matrix row and columns:

- Upper switch: `P1.06` (row) to `P1.00` (column), global `RC(4,9)`.
- Lower switch: `P1.06` (row) to `P1.04` (column), global `RC(4,11)`.

Keep the existing `col2row` diode direction. Both halves use 29 addressable
RGB LEDs after adding one LED for each new right thumb key.

Flash the `settings_reset` image once before installing this firmware so an
older ZMK Studio layout cannot override the new 58-key layout.
