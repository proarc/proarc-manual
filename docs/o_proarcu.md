# ProArc

ProArc je open-source systém pro tvorbu popisných, technických a administrativních metadat pro digitalizované i born-digital dokumenty. 

Podporuje [standardy Národní digitální knihovny (NDK)](https://standardy.ndk.cz/) a produkuje data kompatibilní se systémem [Kramerius](https://github.com/ceskaexpedice/kramerius).

Systém je volně dostupný pod licencí [GNU GPLv3](https://github.com/proarc/proarc/blob/master/LICENSE.txt) a skládá se z:

- [jádra](https://github.com/proarc/proarc/) ([technická dokumentace](https://github.com/proarc/proarc/wiki)),
- [klientské aplikace](https://github.com/proarc/proarc-client/) ([technická dokumentace](https://github.com/proarc/proarc-client/wiki)).

**Poslední stabilní verze**

* [Jádro 4.2.10](https://github.com/proarc/proarc/releases/tag/v4.2.10),
* [Klient 2.3.5](https://github.com/proarc/proarc-client/releases/tag/v2.3.5).

## Podporované typy dokumentů
Systém v současnosti podporuje popis a zpracování:

- periodik,
- monografií,
- zvukových dokumentů (gramofonové desky, fonografické válečky),
- elektronických periodik a monografií,
- starých tisků, včetně konvolutů.

## Funkce systému
- Evidence digitalizačního workflow.
- Import skenů, konverze do JPG2000, prioritizace importu, správa zařízení.
- Generování UUID
- Popis skenů a celého dokumentu s uživatelsky volitelným nastavením obrazovek.
- Převedení katalogizačního záznamu MARC → MODS, editace metadat.
- Vyhledávání v metadatech.
- Kontrolní a validační mechanismy přímo v uživatelském rozhraní.
- Různé druhy exportů (FOXML, NDK PSP, Archivní export, BagIt), přímé importy do připojeného systému Kramerius.
- Podpora stávajících datových modelů systému Kramerius.
- Import NDK PSP nebo FOXML ze systému Kramerius.
- Možnost nahrazovat jednotlivé datastreamy (možnost výměny jednotlivých stran se zachováním UUID).
- Rozšířená komunikace s resolverem URN:NBN (možnost deaktivace, registrace následovníka dokumentu apod.).
- Tvorba nového ALTO/OCR pomocí [Projektu PERO OCR](https://pero-ocr.fit.vutbr.cz/index).
- Převod PDF dokumentů do archivního formátu PDF/A.
- Doplnění odkazu na digitalizovaný dokument do knihovního katalogu.
- Volitelná barevnost aplikace.

## Technologie

  * Open-source řešení (licence GNU GPLv3)
  * Fedora Commons repository >> Akubra
  * Java
  * PostgreSQL
  * Kakadu - použití pro vytvoření JPG2000. Pro získání instalace určené pro využití v ProArcu pro nekomerční účely je možné kontaktovat Národní knihovnu ČR - Bc. Petru Burdovou ([petra.burdova@nkp.cz](mailto:petra.burdova@nkp.cz)).

Systémy, které navazují nebo poskytují dostupnou funkcionalitu
 - Systém Kramerius [https://github.com/ceskaexpedice/kramerius](https://github.com/ceskaexpedice/kramerius)

