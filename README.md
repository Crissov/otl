OTL: OpenType Layout features
====

The `.fea` files contained in this repository follow [standard Adobe feature file syntax](https://www.adobe.com/devnet/opentype/afdko/topic_feature_file_syntax.html) and names from the [Adobe glyph list for new fonts (AGLFN)](https://sourceforge.net/adobe/aglfn/wiki/Home/). They should be usable in most current font editors, but authors may need to adjust feature and glyph names to suit their design.

`rnum`: Roman numerals
----
Using the code from a [Typohile thread](http://typophile.com/node/67366) there are two variants for `ss09` that transform numbers with standard digits to roman numerals, e.g. `4` → `IV`. Variant 1 was posted by Igor Freiberger and variant 2 is by Michael Hernan.

`rmnz`: Romanize
----
This non-standard feature shows characters from non-roman scripts (currently Greek and Cyrillic) with Latin glyphs, using respective ISO standards (which usually only cover contemporary letters).
