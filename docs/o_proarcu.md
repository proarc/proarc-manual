# ProArc

ProArc je open-source systém pro tvorbu popisných, technických a administrativních metadat pro digitalizované i born-digital dokumenty. 

Podporuje [standardy Národní digitální knihovny (NDK)](https://standardy.ndk.cz/) a produkuje data kompatibilní se systémem [Kramerius](https://github.com/ceskaexpedice/kramerius).

Systém je volně dostupný pod licencí [GNU GPLv3](https://github.com/proarc/proarc/blob/master/LICENSE.txt) a skládá se z:

- [jádra](https://github.com/proarc/proarc/) ([technická dokumentace](https://github.com/proarc/proarc/wiki)),
- [klientské aplikace](https://github.com/proarc/proarc-client/) ([technická dokumentace](https://github.com/proarc/proarc-client/wiki)).

!!! info "Aktuální verze ProArcu"

    === "4.3.x"

        - **Implementace nových Definic metadatových formátů (DMF)** se zaměřením na elektronické publikace.
        - **Optimalizace uživatelské práce a rozhraní** pro rychlejší paginaci, přehlednější správu importů a flexibilnější práci s uživatelskými rolemi.
        - **Optimalizace interních procesů** a rozšíření možností hromadných operací nad daty.

        [:octicons-arrow-right-24: Zobrazit přehled hlavních změn](./changelog/v43x.md)

    === "5.0.x"
            
        - **Zahrnuje úpravy z předchozích verzí**
        - **Navíc obsahuje upgrade softwarových komponent**:
            - modernizaci softwarového jádra (přechod na Javu 21), 
            - kontejnerizaci aplikace (Docker).

        [:octicons-arrow-right-24: Zobrazit přehled hlavních změn](./changelog/v50x.md)

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
  * Kakadu - použití pro vytvoření JPG2000.

Systémy, které navazují nebo poskytují dostupnou funkcionalitu
 - Systém Kramerius [https://github.com/ceskaexpedice/kramerius](https://github.com/ceskaexpedice/kramerius)

