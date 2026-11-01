# Construction sheet

The flag's shape is set by the table attached to the Turkish Flag Law, Law No. 2893 (Türk Bayrağı Kanunu, accepted 22/9/1983, Resmî Gazete 24/9/1983, no. 18171). It replaced the first flag law, No. 2994 of 29 May 1936. Article 2: the Turkish flag is the white crescent-and-star red flag, in the shapes and proportions shown in the attached table. The table's note: whatever the flag's width, the G ratios don't change.

The official drawing and table: [official-table.png](official-table.png). Translated, with letters as in the law and each value in vector units where G = 60000:

| Letter | Official text | Meaning | Value | Vector units |
|---|---|---|---|---|
| G | Genişlik | Width of the flag (height along the pole) | G | 60000 |
| A | Ayın dış çemberi merkezinin uçkurluktan uzaklığı | Distance from the hem to the centre of the outer crescent circle | 1/2 G | 30000 |
| B | Ayın dış çemberinin çapı | Diameter of the outer crescent circle | 1/2 G | 30000 (r 15000) |
| C | Ayın iç ve dış çemberlerinin merkezleri arasındaki uzaklık | Distance between the centres of the inner and outer crescent circles | 0.0625 G | 3750 |
| D | Ayın iç çemberinin çapı | Diameter of the inner crescent circle | 0.4 G | 24000 (r 12000) |
| E | Yıldız çemberinin ayın iç çemberinin uçkurluk yönünde ekseni kestiği noktaya uzaklığı | Distance from the star's circle to the point where the inner crescent circle crosses the centre line on the hem side | 1/3 G | 20000 |
| F | Yıldız çemberinin çapı | Diameter of the star's circle | 1/4 G | 15000 (r 7500) |
| L | Boy | Length of the flag | 1 1/2 G | 90000 |
| M | Uçkurluk genişliği | Width of the hem (the white sleeve at the pole) | 1/30 G | 2000 |

Some English sources reorder these letters. The ones above are the law's.

## How the vector follows from it

- Outer circle: centre (30000, 0), radius 15000.
- Inner circle: centre (33750, 0), radius 12000.
- The circles meet at (42675, ±8021), rounded to whole units. Check: 12675² + 8021² ≈ 15000² and 8925² + 8021² ≈ 12000².
- E runs from the inner circle's hem-side crossing of the centre line (33750 - 12000 = 21750) to the star's circle (49250 - 7500 = 41750): 20000 = G/3.
- Star circle: centre (49250, 0), radius 7500. One point at (41750, 0) aims at the crescent. The others sit at 72° steps: (46932, ±7133) and (55318, ±4408).
- The star is a regular five-pointed star whose points lie on that circle.

## The white hem

M is the white sleeve (uçkurluk) at the pole, marked BEYAZ next to the red (AL) field in the official drawing. A is measured from the hem, so the vector's x = 0 is the seam between hem and red. Screen and print drawings, including the reference vector, usually leave the hem out. When you need the physical flag's full layout, add a white strip 2000 units wide on the pole side (x -2000 to 0) and keep everything else where it is.

## Colour

Law No. 2893 and its table say "al" (red) and "beyaz" (white) but give no colour code. Cloth and dye details are left to the regulation (Türk Bayrağı Yönetmeliği) and the Turkish Standards Institution standard for flag cloth (TS 1).

For screens use `#E30A17` (RGB 227, 10, 23). It's the value in the Wikimedia vector and the one most Turkish sources give, and it's close to Pantone 186 C. Some flag books list other Pantone references (2035 C, 032), and commercial colour sites list values like `#C8102E`. Treat those as approximations and stay with `#E30A17` unless the user's brand guide says otherwise. White is pure white.

## Sources

- Law No. 2893, Türk Bayrağı Kanunu, official text with the construction table: mevzuat.gov.tr, `https://www.mevzuat.gov.tr/mevzuatmetin/1.5.2893.pdf`.
- Wikimedia Commons, `File:Flag_of_Turkey.svg` (the path data in this skill).
