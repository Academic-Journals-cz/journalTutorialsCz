# Rozšíření našich časopisů v OJS

Vzhled časopisů netvoří jen samotná šablona webu Academic Journals Cz. Spolu s ní pracuje sada doplňků (pluginů), které
na stránky přidávají údaje o časopisu, statistiky a metriky, plné texty nebo odkazy na sociální sítě.
ˇÚdaje se doplňují do pluginů společně s redakcí – čím úplnější údaje jsou,
tím víc toho web o časopisu ukáže.

Následující přehled shrnuje, co jednotlivé doplňky dělají a co z nich redakce má.

---

## Bloky v postranním panelu

### Indexace v databázích (journalDbFinderAj)

Postranní blok, který ukazuje, ve kterých databázích je časopis indexován. Aktuálně jsou v pluginu nasazeny tyto databáze a indexační nástroje: DOAJ, Scopus,
Web of Science, Crossref, OpenAIRE, CEEOL, CORE, Dimensions, GoTriple, OpenAlex, Semantic Scholar, Dimond Discovery Hub, FatCat, ERIH+, EBSCO
PubMed, ROAD a Redalyc. V části databází se časopis vyhledává automaticky pomocí akce v pluginu, a to podle názvu
časopisu **i** ISSN zároveň. U databází, které automatické vyhledávání neumožňují se pak dá přidat odkaz na databázi ručně
U každé nalezené databáze se zobrazí logo s odkazem přímo na záznam časopisu v blokovém pluginu.

### O časopisu (journalInfoAj)

Postranní blok se základními údaji z pluginu Context Enhancer: šéfredaktor, periodicita, rok založení,
forma vydávání a klíčová slova. Zobrazí se pouze vyplněné – nevyplněné se přeskočí a prázdný blok se vůbec neukáže.

---

## Doplňky na stránkách časopisu a článků

### Statistiky a metriky (citationMetricsAj)

Na stránce článku zobrazí dlaždice s počtem citací ze tří zdrojů: **Crossref Cited-by**,
**Scopus Cite Score**, **Web of Science InCites**, **citace v OpenAlex**, **citace v Semantic Scholars** a proklik na vyhledání článku v **Google Scholar**. U Crossrefu se po kliknutí rozbalí seznam prací, které článek citují; u Scopusu, Web of Science, OpenAlex a Semantic Scholar dlaždice odkazuje na záznam v dané databázi.

Zdroj se zapne tím, že se k němu vyplní přístupové údaje – bez nich se dlaždice nezobrazí.
Výsledky se ukládají a obnovují jednou týdně, takže stránka článku nemusí načítat data opakovaně a zůstává rychlá.

### Doplňková metadata časopisu (contextEnhancerAj)

Rozšiřuje nastavení časopisu o údaje, které OJS sám nenabízí: fakulta, univerzita, obor
podle klasifikace OECD, DOI časopisu, klíčová slova, databáze, SJR, Impact Factor,
forma vydávání, šéfredaktor, periodicita, rok založení nebo informace o tom, že
časopis vychází i mimo naši platformu s odkazem na něj.

Je to **hlavní zdroj údajů pro celý web**: čerpá z něj portál časopisů (filtrování
a řazení, karty časopisů), blok „O časopisu" i další části stránek. Vyplatí se proto
mít tyto údaje kompletní a aktuální.

### Plný text v HTML (inlineHtmlGalleyAj)

Pokud má článek plný text v HTML, zobrazí se přímo na stránce článku jako záložka
„Plný text" – ve vzhledu webu a bez vnořeného rámu, ve kterém bylo dřív nutné rolovat
zvlášť. Původní soubor zůstává beze změny.

### Nabídka obsahu v e-mailech (insertContentAj)

Upravuje nabídku „Vložit obsah" v e-mailových šablonách tak, aby v ní byly jen položky,
které redakce opravdu potřebuje (například posudky). Šablony e-mailů se tím zpřehlední.

### Nově publikováno (latestIssues)

Dodává na úvodní stránku portálu přehled nedávno vydaných čísel napříč všemi časopisy.
Čerstvě vydané číslo se tak objeví na portálu bez jakéhokoli zásahu redakce.

### Sociální sítě (socialLinksAj)

Do nastavení časopisu přidá pole pro odkazy na sociální sítě a profily; v zápatí se pak
zobrazí jako ikony. Vedle běžných sítí podporuje i akademické – ResearchGate, ORCID,
Google Scholar, Academia.edu, Zenodo a další. Vyplní se jen to, co časopis skutečně má.

---

## Doplňky pro viditelnost a indexaci

Následující pluginy vznikly v evropském projektu **CRAFT-OA** a jsou zaměřené
na dohledatelnost časopisů v databázích a službách.

### Discoverability Companion (disco)

Přehled požadavků, které na časopisy kladou databáze, indexační a agregační databáze (DOAJ, Scopus
a další), sestavený do jednoho srozumitelného seznamu. Část kritérií si OJS ověří sám
(například zda má časopis popis nebo zda vychází pravidelně), zbytek redakce zaškrtne.
Plugin pak ukáže, do kterých databází je časopis připraven se přihlásit a co ještě chybí
doplnit; u splněných služeb nabídne přímý odkaz na přihlášku. Umí také zobrazit odznaky
na titulní stránce časopisu (například Diamond OA nebo přidělování DOI).

**Pozn.:** tento plugin je dostupný pouze v angličtině.

### OpenAIRE (openAIRE)

Zajišťuje, aby metadata článků odpovídala pravidlům OpenAIRE (Guidelines v4) a propisovala
se do databáze OpenAIRE Graph – jedné z největších evropských databází výzkumných výstupů,
napojené na European Open Science Cloud. Prakticky to znamená lepší dohledatelnost článků
a možnost přiřadit sekcím časopisu správný typ dokumentu.

### Výměna metadat časopisu (jmef)

Zpřístupní metadata časopisu ve formátu JMEF (Journal Metadata Exchange Format), který
vznikl v projektu CRAFT-OA a využívá ho především Diamond Discovery Hub (DDH). Služby si tak
mohou údaje o časopisu stáhnout automaticky, bez ručního vyplňování formulářů. Důležitý pro napojení do DDH.

---

## Přístup k pluginům

Z bezpečnostních důvodů bude správa doplňků v OJS nadále přístupná **pouze administrátorovi**. Nastavení jednotlivých doplňků i jejich zapínání a vypínání tedy zajišťuje
administrátor, nikoli redakce. Důvodem je, že některé pluginy zasahují do metadat,
exportů a napojení na externí služby, kde by neuvážená změna mohla ovlivnit indexaci
časopisu nebo odeslaná data.

Pokud budete cokoli potřebovat – zapnout doplněk, upravit jeho nastavení, doplnit
přístupové údaje k citačním službám nebo jen poradit, co která volba znamená – obraťte se
prosím na administrátora platformy. Rád vám s tím pomůže.
