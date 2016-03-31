OTL: OpenType Layout features
====

The `.fea` files contained in this repository follow [standard Adobe feature file syntax](https://www.adobe.com/devnet/opentype/afdko/topic_feature_file_syntax.html) and names from the [Adobe glyph list for new fonts (AGLFN)](https://github.com/adobe-type-tools/agl-aglfn/). They should be usable in most current font editors, but authors may need to adjust feature and glyph names to suit their design.

`rnum`: Roman numerals
----
Using the code from a [Typohile thread](http://typophile.com/node/67366) there are two variants for `ss09` that transform numbers with standard digits to roman numerals, e.g. `4` → `IV`. Variant 1 was posted by Igor Freiberger and variant 2 is by Michael Hernan.

`rmnz`: Romanize
----
This non-standard feature shows characters from non-roman scripts with Latin glyphs, using respective ISO standards (which usually only cover contemporary letters).

Implemented (but hardly tested):

- `lookup CyrillicRomanization`: ISO 9:1995
- `lookup GreekRomanization`: ISO 843:1997
- `lookup HebrewRomanization`: ISO 259-1:1984, ISO 259-2:1994, ISO 259-3:1999
- `lookup ArabicRomanization`: ISO 233-1:1984 (not DIN 31635:2011-07)

Planned:

- `lookup ArmenianRomanization`: ISO 9985
- `lookup GeorgianRomanization`: ?
- `lookup ThaiRomanization`: ISO 11940
- `lookup DevanagariRomanization` (and other Indian scripts): ISO 15919
- `lookup KanaRomanization` (Katakana, Hiragana): ISO 3602 (Strict) “Nihon-siki”
- `lookup PinyinRomanization` (Chinese): ISO 7098
