# Maargam Bible versions (downloads)

Optional Bible versions for the Maargam app (Settings > More Bible versions). Each file is a
read-only SQLite database holding one New Testament, **unedited**, built from the eBible.org
archive named below by `npm run build:packs` in the Maargam source repository. The app
downloads a file from `packs-1/` and uses it only if its size and SHA-256 equal the catalog
compiled into the app (`SHA256SUMS` here lists the same hashes).

| File | Version | Language | Licence | Source |
|---|---|---|---|---|
| `packs-1/eng-bsb-1.sqlite` | Berean Standard Bible (BSB) | English | Public domain | eBible.org `engbsb` |
| `packs-1/eng-kjv-1.sqlite` | King James Version (1769) | English | Public domain (outside the UK; Crown letters patent apply to printing in the UK) | eBible.org `eng-kjv` |
| `packs-1/eng-asv-1.sqlite` | American Standard Version (1901) | English | Public domain | eBible.org `eng-asv` |
| `packs-1/tel-otcv-1.sqlite` | Biblica® Open Telugu Contemporary Version™ (OTCV) | Telugu | CC BY-SA 4.0 | eBible.org `telotsa` |

**OTCV attribution (CC BY-SA 4.0):** Biblica® Open Telugu Contemporary Version™, Copyright
© 1976, 1990, 2022, 2024 by Biblica, Inc. Licensed under the Creative Commons
Attribution-ShareAlike 4.0 International License
(https://creativecommons.org/licenses/by-sa/4.0/). Text unmodified (verse text extracted
from USFM; notes and headings omitted). "Biblica" is a trademark of Biblica, Inc. The
original is available free at biblica.com and open.bible.

Each version's own copyright page, as shipped in its archive, is in `licenses/`.

Only versions whose licence allows free redistribution are published here. Copyrighted
versions (for example NKJV, BSI Telugu) are not, unless their rights holders grant written
permission.

Files are never replaced: a new edition gets a new folder (`packs-2/`), so a hash in an
installed app always refers to the same bytes.
