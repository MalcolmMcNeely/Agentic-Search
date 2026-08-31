# Hero files

> **Covers:** one line per hero owned, pointing at that hero's full kit file.
> **Updated:** 2026-08-31

The second hop of the index. [../../INDEX.md](../../INDEX.md) points here; this file points at one of 43 hero files. Read the row, then open only the files the comp actually needs.

Every hero file carries the same five fields, so grep works across the folder:

```
grep -l "Damage:\*\* Magic" mechanics/heroes/*.md
grep -l "Class:\*\* Tank" mechanics/heroes/*.md
```

| Hero | Faction | Class | Damage | Range | Level | File |
| --- | --- | --- | --- | --- | --- | --- |
| Aurora | Celestial | Mage | Magic | 2, or 3 with Enhance Force | S | [aurora.md](aurora.md) |
| Rolan | Celestial | Support | Magic | 10 | S | [rolan.md](rolan.md) |
| Elijah & Lailah | Celestial | Support | Magic | 6 | S | [elijah-lailah.md](elijah-lailah.md) |
| Yamato & Gabumon | Dimensional | Mage | Magic | not published | S | [yamato-gabumon.md](yamato-gabumon.md) |
| Pandora | Dimensional | Support | Magic | 5 | S | [pandora.md](pandora.md) |
| Taichi & Agumon | Dimensional | Warrior | Physical | 7 before digivolve, 1 after | S | [taichi-agumon.md](taichi-agumon.md) |
| Shemira | Graveborn | Mage | Magic | 4 | S | [shemira.md](shemira.md) |
| Viperian | Graveborn | Mage | Magic | 5 | A | [viperian.md](viperian.md) |
| Bonnie | Graveborn | Marksman | Magic | 7 | A | [bonnie.md](bonnie.md) |
| Cecia | Graveborn | Marksman | Physical | 5 | S | [cecia.md](cecia.md) |
| Shadewing | Graveborn | Rogue | Magic | 1 | A | [shadewing.md](shadewing.md) |
| Daimon | Graveborn | Tank | Magic | 3 | A `unverified` | [daimon.md](daimon.md) |
| Valka | Graveborn | Warrior | Physical | 1 | A | [valka.md](valka.md) |
| Phraesto | Hypogean | Tank | Magic | 1 | S | [phraesto.md](phraesto.md) |
| Cyran | Lightbearer | Mage | Magic | 6 | S | [cyran.md](cyran.md) |
| Mirael | Lightbearer | Mage | Magic | 3 | A | [mirael.md](mirael.md) |
| Rowan | Lightbearer | Mage | Magic | 3 | A | [rowan.md](rowan.md) |
| Silven | Lightbearer | Marksman | Physical, with a true damage component | ranged, exact tiles not published | A | [silven.md](silven.md) |
| Zanie | Lightbearer | Marksman | Physical | 20 | A | [zanie.md](zanie.md) |
| Fay | Lightbearer | Support | Magic | 3 | A | [fay.md](fay.md) |
| Hammie | Lightbearer | Support | Magic | 5 | Rare | [hammie.md](hammie.md) |
| Hugin | Lightbearer | Support | Physical | 20 | A | [hugin.md](hugin.md) |
| Chippy | Lightbearer | Tank | Physical | 1 | Rare | [chippy.md](chippy.md) |
| Temesia | Lightbearer | Tank | Physical | 1 | S | [temesia.md](temesia.md) |
| Lucius | Lightbearer | Warrior | Physical | 1 | A | [lucius.md](lucius.md) |
| Valen | Lightbearer | Warrior | Physical | 1 | A | [valen.md](valen.md) |
| Galahad | Mauler | Mage | Magic | 10 | S | [galahad.md](galahad.md) |
| Seth | Mauler | Rogue | Physical | 1 | A | [seth.md](seth.md) |
| Koko | Mauler | Support | Physical | 4 | A | [koko.md](koko.md) |
| Smokey & Meerky | Mauler | Support | Magic | 8 | S | [smokey-meerky.md](smokey-meerky.md) |
| Antandra | Mauler | Tank | Physical | 1 | A | [antandra.md](antandra.md) |
| Gerda | Mauler | Tank | Physical | 1 | A | [gerda.md](gerda.md) |
| Kordan | Mauler | Warrior | Physical | 1 | A | [kordan.md](kordan.md) |
| Kruger | Mauler | Warrior | Physical | 1 | A | [kruger.md](kruger.md) |
| Arden | Wilder | Mage | Magic | 5 | A | [arden.md](arden.md) |
| Eironn | Wilder | Rogue | Magic | 1 | S | [eironn.md](eironn.md) |
| Lily May | Wilder | Rogue | Magic | 3 | S | [lily-may.md](lily-may.md) |
| Faramor | Wilder | Rogue | Physical | 1 | A | [faramor.md](faramor.md) |
| Lenya | Wilder | Rogue | Physical | 1 | A | [lenya.md](lenya.md) |
| Hewynn | Wilder | Support | Magic | 4 | S | [hewynn.md](hewynn.md) |
| Solise | Wilder | Support | Magic | 6 | S | [solise.md](solise.md) |
| Velara | Wilder | Support | Magic | 5 | S | [velara.md](velara.md) |
| Thador | Wilder | Tank | Physical | 1 | A | [thador.md](thador.md) |

## Source

Every row comes from that hero's page on https://www.afk.global/afk-journey/characters/. Conflicts with other sources are recorded in the hero file itself.
