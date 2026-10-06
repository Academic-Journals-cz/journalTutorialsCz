# Rozšíření našich časopisů v OJS

Vzhled a funkce časopisů netvoří jen samotná šablona webu Academic Journals Cz. Spolu s ní pracuje sada doplňků (pluginů), které na stránky přidávají údaje o časopisu, indexaci v databázích, citační metriky, plné texty nebo odkazy na sociální sítě. Většina z nich čerpá z údajů, které o časopisu vyplníme – **čím úplnější údaje jsou, tím víc toho web o časopisu ukáže a tím snáz ho čtenáři i databáze najdou.**

Následující přehled shrnuje, co jednotlivé doplňky dělají, kde je na webu uvidíte a co z nich redakce má.

---

## Souhrn

| Doplněk | Co přináší | Kde ho uvidíte | Kdo ho nastavuje |
|---|---|---|---|
| Doplňková metadata časopisu | údaje o časopisu nad rámec OJS | portál (karty a filtry), blok „O časopisu" | administrátor s redakcí |
| Indexace v databázích | 18 databází, 13 z nich prohledává automaticky | postranní panel, karty a filtr portálu | administrátor |
| O časopisu | základní údaje o časopisu | postranní panel | (čerpá z doplňkových metadat) |
| Citační metriky | počty citací ze 6 zdrojů | stránka článku | administrátor |
| Odkazy u referencí | DOI a Google Scholar u každé reference | stránka článku | funguje samo |
| Plný text v HTML | plný text přímo na stránce článku | stránka článku | funguje samo |
| Sociální sítě | až 29 sítí a profilů | zápatí webu | **redakce sama** |
| GitHub stránky | stránky z dokumentů na GitHubu | vlastní stránky časopisu | **redakce sama** |
| Nově publikováno | nejnovější čísla všech časopisů | úvodní stránka portálu | funguje samo |
| Nabídka obsahu v e-mailech | přehlednější e-mailové šablony | e-maily v redakčním systému | administrátor |
| Discoverability Companion, OpenAIRE, JMEF | viditelnost a indexace (projekt CRAFT-OA) | nastavení, exporty metadat | administrátor |

---

## Údaje o časopisu a jeho viditelnost

POZN. Některá data na obrázcích jsou smyšlená a jsou pouze ilustrativní. Nemusí nutně korespondovat s aktuálním reálným nastavením časopisů! Zároveň funkgují všechny níže popsané pluginy napříč všemi variantami vizuálu Academic Journals Cz. Pro ilustraci byla vybrána základní podoba UPOL, ale vše koresponduje vybranému konkrétnímu vizuálu.

### Doplňková metadata časopisu (contextEnhancerAj)

Rozšiřuje nastavení časopisu o údaje, které OJS sám nenabízí:

- univerzita a fakulta,
- obor podle klasifikace OECD,
- DOI časopisu a klíčová slova,
- databáze, ve kterých je časopis indexován,
- metriky SJR a Impact Factor,
- forma vydávání (tištěný, online, tištěný i online),
- šéfredaktor, periodicita a rok založení,
- informace o tom, že časopis vychází i mimo naši platformu, s odkazem na jeho web.

Je to jeden z **hlavních zdrojů údajů pro celý web.** Z těchto údajů se skládají tři věci, které čtenáři vidí nejčastěji:

**Filtry na portálu časopisů.** Návštěvník portálu si může časopisy vyfiltrovat podle fakulty, oboru OECD, formy vydávání, databází a omezit je rozsahem Impact Factoru a SJR. Časopisy pak může řadit abecedně, podle Impact Factoru, podle SJR nebo podle fakulty. Filtry podle jazyka a licence se berou z běžného nastavení OJS.

![Filtry na portálu časopisů](/images/plugins/01-portal-filters.png)
*Obrázek 1: Údaje z doplňkových metadat se na portálu propisují do filtrů.*

**Karty časopisů na portálu.** Každá karta ukazuje fakultu (v barvě fakulty), rok založení, periodicitu, jazyk, formu vydávání, databáze a metriky IF a SJR.

![Karta časopisu na portálu](/images/plugins/02-portal-journal-summary.png)
*Obrázek 2: Karta časopisu na portálu – většina údajů pochází z doplňkových metadat.*

**Blok „O časopisu" v postranním panelu** – viz níže.

Vyplatí se proto mít tyto údaje kompletní a aktuální; s doplněním vám rád pomůže administrátor platformy.

### Indexace v databázích (journalDbFinderAj)

Postranní blok na stránkách časopisu, který ukazuje, **ve kterých databázích je časopis indexován.** U každé databáze se zobrazí její logo s odkazem přímo na záznam časopisu v dané databázi.

Plugin pracuje s **18 databázemi a indexačními službami.** Ve **13 z nich časopis vyhledá automaticky**:

- DOAJ, Scopus, Web of Science, Crossref, OpenAlex, OpenAIRE, Semantic Scholar, CORE, Dimensions, PubMed, Fatcat, ROAD a Diamond Discovery Hub.

Časopis se vždy hledá **podle ISSN (kde je to možné) i podle názvu **. Výsledky se pravidelně samy obnovují; když je některá databáze zrovna nedostupná, zůstane zobrazen poslední známý výsledek.

U **pěti databází**, které automatické vyhledávání neumožňují (nemají veřejné rozhraní), se odkaz na záznam časopisu vkládá ručně: **CEEOL, GoTriple, Redalyc, ERIH PLUS a EBSCO.** Pokud je v některé z nich váš časopis, pošlete administrátorovi odkaz na jeho záznam.

![Blok s databázemi v postranním panelu](/images/plugins/03-db-finder-block.png)
*Obrázek 3: Postranní blok s logy databází; každé logo vede na záznam časopisu v databázi.*

Ověřené databáze se navíc zobrazují **i na kartě časopisu na hlavní stránce portálu** (jako odkazy) a dá se podle nich **filtrovat**.

### O časopisu (journalInfoAj)

Postranní blok se základními údaji z doplňkových metadat: šéfredaktor, periodicita, rok založení, forma vydávání a klíčová slova. Zobrazí se pouze vyplněné údaje – nevyplněné se přeskočí a prázdný blok se vůbec neukáže.

![Blok O časopisu](/images/plugins/04-about-journal-block.png)
*Obrázek 4: Blok „O časopisu" v postranním panelu.*

---

## Články a jejich dopad

### Citační metriky (citationMetricsAj)

Na stránce článku zobrazí dlaždice s tím, **kolikrát byl článek citován v konrétních databázích.** Plugin citace kontroluje podle **DOI článků**:

- **Crossref Cited-by** – počet citací; po kliknutí se rozbalí seznam prací, které článek citují,
- **Scopus** – počet citací s odkazem na citující dokumenty ve Scopusu,
- **Web of Science** – počet citací s odkazem na záznam ve Web of Science,
- **OpenAlex** – počet citací s odkazem na seznam citujících prací,
- **Semantic Scholar** – počet citací s odkazem na citující práce,
- **Google Scholar** – odkaz na vyhledání článku (Google Scholar nemá veřejné rozhraní, takže počet citací ukázat nejde; čtenář ho uvidí po prokliku).

Podmínkou je, aby **článek měl přidělené DOI** – bez něj citace dohledat nejde. Výsledky se ukládají a obnovují jednou týdně, takže stránka článku nemusí načítat data opakovaně a zůstává rychlá. Každou dlaždici lze v nastavení vypnout; Crossref, Scopus a Web of Science potřebují přístupové údaje, které nastavuje administrátor, OpenAlex, Semantic Scholar a Google Scholar fungují bez nich.

![Dlaždice s citacemi](/images/plugins/05-bibliometrics.png)
*Obrázek 5: Dlaždice s počty citací z jednotlivých zdrojů.*

![Rozbalený seznam citujících prací](/images/plugins/06-bibliometrics-crossref.png)
*Obrázek 6: Po kliknutí na Crossref se zobrazí seznam prací, které článek citují.*

### Odkazy u referencí (referenceLinksAj)

Pod každou referenci v seznamu literatury přidá dvě tlačítka: **„Přejít na DOI"**, pokud reference obsahuje DOI, a **„Vyhledej v Google Scholar"**. Čtenář tak citovanou práci otevře jedním kliknutím, místo aby ji ručně dohledával.

Redakce nemusí nic nastavovat – DOI plugin v textu reference rozpozná sám, ať je zapsané jako odkaz (https://doi.org/…), nebo jako doi:10.…. U referencí, které spároval Crossref, se použije i DOI nalezené Crossrefem. Vyplatí se proto **uvádět DOI u referencí všude, kde existuje.**

![Tlačítka pod referencemi](/images/plugins/07-references-links.png)
*Obrázek 7: Pod každou referencí je odkaz na DOI a na vyhledání v Google Scholar.*

### Plný text v HTML (inlineHtmlGalleyAj)

Pokud má článek plný text v HTML, zobrazí se přímo na stránce článku jako záložka „Plný text". Text je dobře čitelný i na mobilu a odkazy na poznámky a literaturu fungují uvnitř stránky. Původní soubor zůstává beze změny.

![Plný text na stránce článku](/images/plugins/08-html-fulltext.png)
*Obrázek 8: Plný text v HTML přímo na stránce článku.*

---

## Portál, web časopisu a komunikace

### Sociální sítě (socialLinksAj)

Umožňuje přidat do zápatí webu odkazy na **až 29 sociálních sítí a profilů** v pěti skupinách:

- **sociální sítě:** Facebook, X, Instagram, Threads, Bluesky, Mastodon, LinkedIn, TikTok, Pinterest,
- **video a zvuk:** YouTube, Vimeo, Spotify, Apple Podcasts, SoundCloud,
- **komunity a zprávy:** Telegram, WhatsApp, Discord, Reddit,
- **odborné sítě:** ResearchGate, Academia.edu, ORCID, Google Scholar, Zenodo, Humanities Commons,
- **ostatní:** GitHub, GitLab, Flickr, Wikipedia, RSS.

**Odkazy spravuje redakce sama** – v *Nastavení → Webová stránka* na záložce **Sociální sítě**.

![Záložka Sociální sítě v nastavení](/images/plugins/09-social-links-settings.png)
*Obrázek 09: Správa sociálních sítí v Nastavení → Webová stránka.*

![Ikony sociálních sítí v zápatí](/images/plugins/10-social-links-footer.png)
*Obrázek 10: V zápatí se zobrazí jen sítě, které redakce zadala.*

### GitHub stránky (githubPages)

Zveřejní dokumenty zapsané ve formátu Markdown (.md) uložené na GitHubu jako **samostatné stránky časopisu** – například pokyny pro autory, etické zásady nebo podrobné postupy. Plugin dokument stáhne, převede ho do vzhledu webu (včetně obrázků) a zobrazí na adrese, kterou si zvolíte. Výhoda je, že text se udržuje na jednom místě na GitHubu, třeba i ve spolupráci s dalšími lidmi; po úpravě stačí stránku jedním tlačítkem *Načíst znovu z GitHubu* aktualizovat. Takto mohou být stránky verzovány a udržovány dalšími uživateli i bez nutnosti zásahu přímo do nastavení časopisu.

**Stránky spravuje redakce sama** – v *Nastavení → Webová stránka* na záložce **GitHub stránky**.

![Záložka GitHub stránky v nastavení](/images/plugins/11-github-pages-settings.png)
*Obrázek 11: Správa GitHub stránek v Nastavení → Webová stránka.*

### Nově publikováno (latestIssues)

Dodává na úvodní stránku portálu přehled nedávno vydaných čísel napříč všemi časopisy.

![Nově publikovaná čísla na portálu](/images/plugins/12-latest-issues.png)
*Obrázek 12: Právě vydaná čísla na úvodní stránce portálu.*

### Nabídka obsahu v e-mailech (insertContentAj)

Upravuje nabídku „Vložit obsah" v e-mailových šablonách tak, aby v ní byly jen položky, které redakce opravdu potřebuje (například posudky). Šablony e-mailů se tím zpřehlední.

![Nabídka Vložit obsah v e-mailu](/images/plugins/13-insert-content.png)
*Obrázek 13: Zjednodušená nabídka „Vložit obsah" v e-mailu.*

---

## Přístup k pluginům

Z bezpečnostních důvodů je správa doplňků v OJS – jejich zapínání, vypínání a nastavení na stránce Pluginy – přístupná **pouze administrátorovi**. Důvodem je, že některé pluginy zasahují do metadat, exportů a napojení na externí služby, kde by neuvážená změna mohla ovlivnit indexaci časopisu nebo odeslaná data.

**Výjimkou jsou doplňky, jejichž obsah redakce spravuje sama.** Mají vlastní záložku v *Nastavení → Webövá stránka* a mají k nim přístup všichni, kdo časopis spravují:

- **Sociální sítě** – odkazy na sociální sítě a profily časopisu,
- **GitHub stránky** – stránky časopisu načítané z GitHubu.

Pokud budete potřebovat cokoli dalšího – zapnout doplněk, doplnit údaje o časopisu, poslat odkaz na záznam v databázi, zadat přístupové údaje k citačním službám nebo jen poradit, co která volba znamená – obraťte se prosím na administrátora platformy. Rád vám s tím pomůže.

