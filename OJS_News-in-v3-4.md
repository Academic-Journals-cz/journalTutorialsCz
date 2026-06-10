# Co je nového v OJS 3.4

## Pracovní workflow

OJS 3.4 přináší několik změn v pracovním workflow:

**Nový a vylepšený průvodce odesláním příspěvku.** 

Nyní je možné rozpracovaný příspěvek průběžně ukládat, změnit jeho jazyk a nastavit soubor (komponentu) jako povinný. 

Podrobněji se můžete na úpravy podívat na následujících odkazech: [Odeslání příspěvku](https://docs.pkp.sfu.ca/learning-ojs/3.4/en/authoring#making-a-submission) a nastavení [Komponent](https://docs.pkp.sfu.ca/learning-ojs/3.4/en/settings-workflow#components).


**Lepší proces zaznamenávání redakčních rozhodnutí.** Při zaznamenání rozhodnutí lze do polí kopie / skrytá kopie (CC/BCC) oznámení autorovi přidat libovolný e‑mail a vložit další obsah. Kopii oznámení lze poslat recenzentům na samostatné obrazovce, která používá e‑mailovou šablonu určenou recenzentům a zachovává anonymitu vůči autorům. Podrobnosti viz [Rozhodnutí](https://docs.pkp.sfu.ca/learning-ojs/3.4/en/editorial-workflow#making-the-decision).

**Možnost zrušit fázi nebo recenzní kolo.** Nově lze zrušit omylem zahájené recenzní kolo — pokud už recenzent neodevzdal recenzi. Lze také zrušit celou fázi a vrátit příspěvek do předchozí fáze (např. z redakčních úprav zpět do recenze), volitelně s upozorněním autora na tuto změnu. Podrobnosti viz [Další kolo recenze](https://docs.pkp.sfu.ca/learning-ojs/3.4/en/editorial-workflow#additional-round-of-review).

**Vylepšené nástroje pro e‑mailové šablony.** OJS 3.4 přináší nové nástroje pro psaní e‑mailů, včetně možnosti vytvářet více šablon a přepínat mezi nimi. U každého e‑mailu je přehled dostupných proměnných, které lze vložit tlačítkem „Vložit obsah". Hodnoty proměnných (např. jméno autora) si lze před odesláním zobrazit v náhledu. Výchozí sada e‑mailových šablon byla přepsána tak, aby byla vstřícnější a inkluzivnější. Podrobnosti viz [Nastavení e‑mailů](https://docs.pkp.sfu.ca/learning-ojs/3.4/en/settings-workflow#email-setup).

Sada nástrojů pro redakční rozhodnutí tyto novinky využívá; v dalších verzích se rozšíří i do ostatních částí systému. Více o novém procesu redakčních rozhodnutí najdete v [prezentaci](https://docs.google.com/presentation/d/e/2PACX-1vTpSVv_zY4RShrh3EfBZjHcRSYKVqDkzejDnESh6Bkg7uMgM8zFYZz-ha7j3iz_csTKump2_rI3YNWS/pub#slide=id.g16f0bb3e17f_0_26) a [videozáznamu](https://youtu.be/JEJJ1FVpao0?t=1798).

## Statistiky

Podpora standardu COUNTER byla aktualizována na [COUNTER Release 5](https://www.projectcounter.org/counter-release-5/), včetně nástrojů pro vykazování čtenosti podle regionu a podle institucionálního přístupu. S tím přišla i základní podpora identifikátorů [ROR (Research Organization Registry)](https://ror.org/) pro institucionální předplatné.

> Viz [prezentace](https://docs.google.com/presentation/d/e/2PACX-1vTpSVv_zY4RShrh3EfBZjHcRSYKVqDkzejDnESh6Bkg7uMgM8zFYZz-ha7j3iz_csTKump2_rI3YNWS/pub#slide=id.g16f0bb3e17f_0_44) a [videozáznam](https://youtu.be/JEJJ1FVpao0?t=122).

## Trvalé identifikátory

Podpora identifikátorů DOI a služby CrossRef byla kompletně přepracována — ve spolupráci s CrossRef a s cílem odstranit časté nejasnosti z předchozí verze.

> Viz [prezentace](https://docs.google.com/presentation/d/e/2PACX-1vTpSVv_zY4RShrh3EfBZjHcRSYKVqDkzejDnESh6Bkg7uMgM8zFYZz-ha7j3iz_csTKump2_rI3YNWS/pub#slide=id.g16f0bb3e17f_0_14) a [videozáznam](https://youtu.be/JEJJ1FVpao0?t=501).

## Instalace s více časopisy

Správci webu (Site Administrators) mají nyní stejná manažerská oprávnění jako správci časopisu (Journal Managers), i když roli správce časopisu nemají. Cílem je jasněji oddělit správce webu (často jde o systémové administrátory či technickou podporu, kteří se ale nepodílejí na redakčním procesu) od správců časopisu (kteří se na procesu podílejí). V dřívějších verzích bylo často nutné přiřadit administrátorům obě role. ([GitHub issue #7392](https://github.com/pkp/pkp-lib/issues/7392))

Od verze OJS 3.4.0 mohou správci časopisu řídit zápis uživatelů do svého časopisu bez ohledu na to, zda je uživatel aktivní i v jiných časopisech. Dříve bylo často nutné takové případy předávat správcům webu. ([GitHub issue #7391](https://github.com/pkp/pkp-lib/issues/7391))

## Formátování názvů příspěvků

Názvy příspěvků mohou nyní obsahovat základní formátování — tučné písmo, kurzívu, podtržení, horní a dolní index. To je důležité zejména u článků uvádějících taxonomické názvy (které se obvykle píší kurzívou) a u recenzních článků (které mohou na recenzovaný zdroj odkazovat podtrženým názvem). ([GitHub issue #2564](https://github.com/pkp/pkp-lib/issues/2564))

## Další významné změny

- Fulltextový index příspěvků se už neaktualizuje ve chvíli nahrání souboru. V předchozích verzích to často zdržovalo a bývalo zdrojem frustrace.
- Mezi metadata lze nově zařadit i prohlášení o dostupnosti dat (data availability statement).
- Do systémových e‑mailových oznámení, která to podporují (nové číslo, oznámení, upozornění na diskusi apod.), se nově přidává přímý odkaz „Odhlásit odběr".

## Další informace

Podrobnosti k těmto změnám najdete v prezentaci „December 2022 Development Update" od vývojového týmu PKP — jako [prezentaci](https://docs.google.com/presentation/d/e/2PACX-1vTpSVv_zY4RShrh3EfBZjHcRSYKVqDkzejDnESh6Bkg7uMgM8zFYZz-ha7j3iz_csTKump2_rI3YNWS/pub) a [videozáznam](https://www.youtube.com/watch?v=JEJJ1FVpao0).

## O tomto překladu

Tento text vychází z originálu v dokumentaci PKP: [About Open Journal Systems (OJS) — Learning OJS 3.4](https://docs.pkp.sfu.ca/learning-ojs/3.4/en/about-ojs) (v angličtině).

Pro základní překlad do češtiny byl použit **Claude (model Claude Opus 4.8)** od společnosti Anthropic. Překlad byl následně zkontrolován, doplněn a upraven.