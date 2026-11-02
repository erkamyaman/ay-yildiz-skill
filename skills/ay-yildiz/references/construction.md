# Construction sheet

The flag's shape is set by the table attached to the Turkish Flag Law, Law No. 2893 (Türk Bayrağı Kanunu, accepted 22/9/1983, Resmî Gazete 24/9/1983, no. 18171). Article 10 repeals the earlier flag law, No. 2994 of 29 May 1936. Article 2: the Turkish flag is the white crescent-and-star red flag, in the shapes and proportions shown in the attached table. The table's note: whatever the flag's width, the G ratios don't change.

Details are in the Türk Bayrağı Tüzüğü (No. 85/9034), called "the regulation" here. KHK 700 changed the law's word "tüzük" to "yönetmelik" in 2018, and a transitional article keeps existing tüzükler in force until they're repealed. I found no replacement yönetmelik, so this skill uses the Tüzük.

The official drawing and table: [official-table.png](official-table.png). Translated, with letters as in the law and each value in vector units where G = 60000:

| Letter | Official text | Meaning | Value | Vector units |
|---|---|---|---|---|
| G | Genişlik | Width of the flag (height along the pole) | G | 60000 |
| A | Ayın dış çemberi merkezinin uçkurlurluktan [sic] uzaklığı | Distance from the hem to the centre of the outer crescent circle | 1/2 G | 30000 |
| B | Ayın dış çemberinin çapı | Diameter of the outer crescent circle | 1/2 G | 30000 (r 15000) |
| C | Ayın iç ve dış çemberlerinin merkezleri arasındaki uzaklık | Distance between the centres of the inner and outer crescent circles | 0.0625 G | 3750 |
| D | Ayın iç çemberinin çapı | Diameter of the inner crescent circle | 0.4 G | 24000 (r 12000) |
| E | Yıldız çemberinin ayın iç çemberinin uçkurluk yönünde ekseni kestiği noktaya uzaklığı | Distance from the star's circle to the point where the inner crescent circle crosses the centre line on the hem side | 1/3 G | 20000 |
| F | Yıldız çemberinin çapı | Diameter of the star's circle | 1/4 G | 15000 (r 7500) |
| L | Boy | Length of the flag | 1 1/2 G | 90000 |
| M | Uçkurluk genişliği | Width of the hem (the white sleeve at the pole) | 1/30 G | 2000 |

## How the vector follows from it

- Outer circle: centre (30000, 0), radius 15000.
- Inner circle: centre (33750, 0), radius 12000.
- The circles meet at (42675, ±8021), rounded to whole units. Check: 12675² + 8021² ≈ 15000² and 8925² + 8021² ≈ 12000².
- E runs from the inner circle's hem-side crossing of the centre line (33750 - 12000 = 21750) to the star's circle (49250 - 7500 = 41750): 20000 = G/3.
- Star circle: centre (49250, 0), radius 7500. One point at (41750, 0) aims at the crescent. The others sit at 72° steps: (46932, ±7133) and (55318, ±4408).
- The star is a regular five-pointed star whose points lie on that circle.

## The star's position

The official texts disagree slightly, and no drawing can satisfy both rules.

- E = G/3: the law's table and Article 4(G) of the regulation both give this number. It puts the star's tip at x = 41750.
- Article 4(G) of the regulation also says the tip lies where the centre line meets the line through the crescent's two tips, and the official drawing shows it there. With the table's numbers, that line is at x = 42675.

The two differ by 925 units, about 1.5% of G, and no text says which one wins. This skill follows E = G/3, which is a judgement: it's the stated number in both texts, and the Ministry of National Education's flag pattern guide measures the star this way, from the inner circle's crossing of the centre line. The drawing isn't to scale, and the regulation's size chart has no E column, so neither settles it.

## The white hem

M is the white sleeve (uçkurluk) at the pole, marked BEYAZ next to the red (AL) field in the official drawing. A is measured from the hem's inner edge, so the vector's x = 0 is the seam between hem and red.

Article 2 of the regulation measures the length L from the hem's outer edge to the fly, so L includes the hem. When you need the physical flag's full layout, draw the white hem from x = -2000 to 0, and end the red at x = 88000. The total length stays 90000.

The vector in this skill leaves the hem out for screen use. Its red runs from x = 0 to 90000 to keep the 3:2 shape.

## Colour

Law No. 2893 says "al" (red) and "beyaz" (white) and gives no colour code. Article 3(B) of the regulation (Türk Bayrağı Tüzüğü, as amended 17/7/1995) defines them for cloth:

- Red: lightness 27.5, red-green 44.8, yellow-blue 15.6, with a difference of at most 3 NBS.
- White: twice the reflectance at 460 nm minus the reflectance at 620 nm must be at least 15% for silk and synthetic blends, and at least 60% for other cloth.

The regulation doesn't name the colour scale or the illuminant, so these values have no single exact screen equivalent. Read as CIELAB or Hunter Lab, they convert to a much darker red, roughly `#7F152C` to `#9C1411`. Those are my conversions, not official values. Fabric details are left to a mandatory Turkish Standard, which the regulation doesn't number.

For screens use `#DC0D15`, with white `#FFFFFF`. This is a convention. I found no government source that defines a screen colour for the flag itself, though the Turkish Standard wasn't available to read. `#DC0D15` comes from the Interior Ministry, in two places:

- Its [corporate identity page](https://www.icisleri.gov.tr/kurumsal-kimlik-kilavuz) says its logo uses one colour: "Logoda tek renk, bayrak kırmızısı uygulanmıştır."
- Its [2026 corporate identity guide](https://www.icisleri.gov.tr/kurumlar/icisleri.gov.tr/icerikYonetimi/kurumsal-kimlik/icisleri_bakanligi_kurumsal_kimlik_final_2026.pdf), page 55, lists its main corporate red ("Kurumsal Ana Renk") as `#dc0d15`, Pantone 199 C.

Neither place states both facts, so linking them is an inference, and this is a government identity colour, not a rule about the flag. The [Labour Ministry's guide](https://www.csgb.gov.tr/Media/klghey0a/csgb-kurumsal-kimlik.pdf) lists the same hex. The guide also lists RGB 218 41 28, which is `#DA291C` and doesn't match; this skill uses the hex because it's the value that repeats. The ministry's [2018 guide](https://www.icisleri.gov.tr/kurumlar/icisleri.gov.tr/icisleri/Kurumsal/icisleribakanligi_kurumsalkimlik.pdf) does state both facts, flag red and R 227 G 6 B 19 (`#E30613`), Pantone 185 C, but its current page no longer links that guide. If you need the legal colour, for cloth, use the regulation's coordinates.

## Sources

Government sources only.

- Law No. 2893, Türk Bayrağı Kanunu, with the construction table: mevzuat.gov.tr, `https://www.mevzuat.gov.tr/mevzuatmetin/1.5.2893.pdf`.
- Türk Bayrağı Tüzüğü, No. 85/9034, Articles 2, 3 and 4 and Annexes 1 and 2: mevzuat.gov.tr, `https://www.mevzuat.gov.tr/MevzuatMetin/2.5.859034.pdf`.
- Ministry of National Education, Türk Bayrağı Kalıbı: `https://megep.meb.gov.tr/mte_program_modul/moduller_pdf/T%C3%BCrk%20Bayra%C4%9F%C4%B1%20Kal%C4%B1b%C4%B1.pdf`.
- Interior Ministry, corporate identity page: `https://www.icisleri.gov.tr/kurumsal-kimlik-kilavuz`.
- Interior Ministry, 2026 corporate identity guide, page 55: `https://www.icisleri.gov.tr/kurumlar/icisleri.gov.tr/icerikYonetimi/kurumsal-kimlik/icisleri_bakanligi_kurumsal_kimlik_final_2026.pdf`.
- Labour Ministry, corporate identity guide: `https://www.csgb.gov.tr/Media/klghey0a/csgb-kurumsal-kimlik.pdf`.
- Interior Ministry, 2018 corporate identity guide, printed page 8: `https://www.icisleri.gov.tr/kurumlar/icisleri.gov.tr/icisleri/Kurumsal/icisleribakanligi_kurumsalkimlik.pdf`.
