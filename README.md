Encode::VN Perl
===============

[![CPAN version][version-svg]][version-link]
[![Build Status][build-status-svg]][build-status-link]
[![Docs][docs-metacpan-svg]][docs-metacpan-link]
[![License][license-svg]][license-link]

## NAME

`Encode::VN` - Extra sets of Vietnamese encodings using Unicode Mapping (UCM) files

## VERSION

This document describes version 0.06 of `Encode::VN`, released September 15, 2013.

## SYNOPSIS

```perl
use Encode;
use Encode::VN;
 
# VNI (ANSI)
$vni  = encode("x-viet-vni", $utf8);
$utf8 = decode("x-viet-vni", $vni );
```

## DESCRIPTION

Perl 5.7.3 and later ship with an adequate set of Vietnamese encodings, including the commonly used `VISCII` and `CP1258` (also known as `MacVietnamese`) encodings.

However, there are additional Vietnamese encodings that are used and may be encountered; hence, this CPAN module tries to provide the rest of them.

## ENCODINGS

This version includes the following encoding tables:

Canonical        | Alias             | Description
-----------------|-------------------|-----------------------------------------
x-viet-vni       | /\bVNI(-ANSI)?$/i | VNI ANSI (Win/Unix)
x-viet-vni-ascii | /\bVNI-ASCII$/i   | VNI ASCII (DOS)
x-viet-vni-mac   | /\bVNI-Mac$/i     | VNI Mac
x-viet-vni-email | /\bVNI-Email$/i   | VNI Internet Mail (Win/Unix/Mac)
x-viet-vps       | /\bVPS$/i         | Vietnamese Professionals Society

## SEE ALSO

1. Vietnamese Unicode SourceForge project: http://vietunicode.sourceforge.net/
1. VNI Wikipedia page: http://en.wikipedia.org/wiki/VNI
1. Mozilla VPS mappings: http://lxr.mozilla.org/seamonkey/source/intl/uconv/ucvlatin/vps.uf, http://lxr.mozilla.org/seamonkey/source/intl/uconv/ucvlatin/vps.ut

Encode

## ACKNOWLEDGEMENTS

Maps for `VNI` are generated from the vnichar.htm file, courtesy of the VNI Sofware Comany, http://vnisoft.com/english/vnichar.htm.

Map for `VPS` is generated from the "Unicode & Vietnamese Legacy Character Encodings" page courtesy of the Vietnamese Unicode project on SourceForge, http://vietunicode.sourceforge.net/charset/.

## CONTRIBUTIONS

Any reports of problems, comments or suggestions are most welcome.

Please report these on [Github](https://github.com/grokify/encode-vn-perl)

## AUTHORS

John Wang <johncwang@gmail.com>

## COPYRIGHT

Copyright 2013-2016 by John Wang <johncwang@gmail.com>.

This software is released under the MIT license cited below.

## LICENSE

Encode::VN is available under an MIT-style license. See [LICENSE](LICENSE) for details.

Encode::VN &copy; 2013-2016 by John Wang

 [version-svg]: https://badge.fury.io/pl/Encode-VN.svg
 [version-link]: https://badge.fury.io/pl/Encode-VN
 [build-status-svg]: https://travis-ci.org/grokify/encode-vn-perl.svg?branch=master
 [build-status-link]: https://travis-ci.org/grokify/encode-vn-perl
 [docs-metacpan-svg]: https://img.shields.io/badge/docs-metacpan-blue.svg
 [docs-metacpan-link]: https://metacpan.org/pod/Encode::VN
 [license-svg]: https://img.shields.io/badge/license-MIT-blue.svg
 [license-link]: https://raw.githubusercontent.com/grokify/encode-vn-perl/master/LICENSE