# Hei Arnold film videomäng GBA

## Sohk koodid

Sohkkoodid on tehtud poolt Martin Eesmaa.

**Euroopa prototüüp test ja finaal versioon:**

| Kirjeldus | Kood lõhkuja | Lisateave |
| --- | --- | --- |
| Animatsioon tegelane liigutus menüüs | `0038`* | ? |
| Keeled valimine keskendus | `33001510 0000` (vaikimisi inglise) | 00 - Inglise, 01 - Prantsuse, 02 - Saksa keel |
| Piirkond | `3300168A` | 00: VAIKIMISI (Arnold tänav), 04: NICKI ELUTUBA, 08 - VÄRAV, 0C - FTI EHITUS, 10 - LINNATÄNAV, 14 - HELGA KODU |
| TEGELANE | `3300168C 0000` (vaikimisi päevast Arnold) | 00-01: ARNOLD, 02-03: GERALD, 04-05: VANAISA PHIL, 06-07: VANAEMA GERTIE, 08-09: GERALD BUSS, 0A-0B: HELGA |
| Postkastid? | `1AAC`* | `FFFF33` ei tea? |
| Kollane tomat | `33001AB8 0001` | Aktiveerib saada kollane tomati |
| KESKUNDU HELGA REŽIIM | `33001AD6 0001` | Aktiveerib keskenduda Helga tegelasi |
| Nuppud vajutatud | `1AD8`* | Võid alati vahetada Arnold ja Helga kohta tegelaseid ilma sisestamist saladuskoodi: `28 46 64 82` |
| Jalgpalli pead | `3300239E 0063` | Piiratuta jalgpalli pead |
| Elud | `330023A0 0009` | Piiratuta elud |
| Südad | `3300239C 0005` | Piiratuta südad |
| Hüppa üles | `33004156 0001` | Annab kõrge hüppata |
| Kiirusta üles | `33004157 0001` | Pole lisateavet |
| Võim üles | `33004158 0001` | Pole lisateavet |
| Täht | `3300415D 0001` | Muusika täht algab ja saad ette vaenlased ilma pihta (NB: bossid asemel võib lõhkuda) |
| Punane tomat | `330047C6 0001` | Piiramatu tomatid |
| Paper | `330047C8 0001` | Piiramatu paperid |
| Söörik | `330047CA 0001` | Piiramatu söörikud |
| Korvpall | `330047CC 0001` | Piiramatu korvpallid |
| Tualettpaperid | `330047CE 0001` | Vanaema Gertiel asja |
| Hambad | `330047D0 0001` | Vanaisa Phili asja |
| Näts | `47D2`* | Vaikimisi relv |
| Tundmatu 1 | `5A88`* | Ei klippe, pääse kaudu ja ei saa lüüa paha tegelased (aktiveeri 00) |
| Boss HP elu | `33005C64 0000` | Ainult bossitasemed lõppus |

```text
0038 - Animatsioon tegelane liigutus menüüs
1510 - Keeled valimine (00 - Inglise, 01 - Prantsuse, 02 - Saksa keel)
168A - PIIRKOND (00: VAIKIMISI (Arnold tänav), 04: NICKI ELUTUBA, 08 - VÄRAV, 0C - FTI EHITUS, 10 - LINNATÄNAV, 14 - HELGA KODU)
168C - TEGELANE (00-01: ARNOLD, 02-03: GERALD, 04-05: VANAISA PHIL, 06-07: VANAEMA GERTIE, 08-09: GERALD BUSS, 0A-0B: HELGA)
1AAC - Postkastid? (FFFF33)
1AB8 - Kollane tomat (aktiveeri: 01)
1AD6 - KESKUNDU HELGA REŽIIM (aktiveeri 01)
1AD8 - Nuppud vajutatud (võid alati vahetada Arnold ja Helga kohta tegelaseid ilma sisestamist saladuskoodi: 28 46 64 82)
239E - Jalgpalli pead (00-63 allkirjastatud)
23A0 - Elud (00-09)
239C - Südad (00-05)
4156 - Hüppa üles (aktiveeri: 01)
4157 - Kiirusta üles (aktiveeri: 01)
4158 - Võim üles (aktiveeri: 01)
415D - Täht (aktiveeri: 01)
47C6 - Tomat (aktiveeri: 01)
47C8 - Paper (aktiveeri: 01)
47CA - Söörik (aktiveeri: 01)
47CC - Korvpall (aktiveeri: 01)
47CE - Tualettpaperid (aktiveeri: 01)
47D0 - Hambad (aktiveeri: 01)
47D2 - Näts
5A88 - Ei klippe, pääse kaudu ja ei saa lüüa paha tegelased (aktiveeri 00)
5C64 - Boss HP elu (07-00)
```

- 2026 Martin Eesmaa
