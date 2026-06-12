# Co je nového v OJS 3.4 (Česky)

## Redakční workflow

OJS 3.4 přineslo několik úprav do redakčního workflow:

**Nový a vylepšený průvodce odesláním příspěvku.** 

Nyní je možné rozpracovaný příspěvek průběžně ukládat, změnit jeho jazyk a nastavit soubor (komponentu) jako povinný. 

Podrobněji se můžete na úpravy podívat na následujících odkazech: [Odeslání příspěvku](https://docs.pkp.sfu.ca/learning-ojs/3.4/en/authoring#making-a-submission) a nastavení [Komponent](https://docs.pkp.sfu.ca/learning-ojs/3.4/en/settings-workflow#components).

![Odeslání příspěvku](/images/OJS_News-in-v3-4/submission_process.png)\

**Vylepšený proces zadávání redakčních rozhodnutí.** 

Při zasílání rozhodnutí lze do polí kopie / skrytá kopie (CC/BCC), během přípravy oznámení autorovi, přidat libovolný e‑mail a vložit další obsah. Kopii oznámení lze poslat recenzentům na samostatné obrazovce, která používá e‑mailovou šablonu určenou recenzentům a zachovává anonymitu vůči autorům. Podrobnosti viz [Rozhodnutí](https://docs.pkp.sfu.ca/learning-ojs/3.4/en/editorial-workflow#making-the-decision).

![Zasílání rozhodnutí](/images/OJS_News-in-v3-4/decision_form.png)\

**Možnost zrušit fázi nebo recenzní kolo.** 

Nově lze zrušit omylem zahájené recenzní kolo – pokud už recenzent neodevzdal recenzi. Lze také zrušit celou fázi a vrátit příspěvek do předchozí fáze (např. z redakčních úprav zpět do recenze), volitelně s upozorněním autora na tuto změnu. Podrobnosti viz [Další kolo recenze](https://docs.pkp.sfu.ca/learning-ojs/3.4/en/editorial-workflow#additional-round-of-review).

![Zrušení fáze](/images/OJS_News-in-v3-4/cancel_stage.png)\

**Vylepšené nástroje pro úpravu šablon e‑mailů.** 

OJS 3.4 přináší nové nástroje pro úpravu e‑mailů, včetně možnosti vytvářet více šablon a přepínat mezi nimi. U každého e‑mailu je přehled dostupných proměnných, které lze vložit tlačítkem „Vložit obsah". Hodnoty proměnných (např. jméno autora) si lze před odesláním zobrazit v náhledu. Výchozí sada e‑mailových šablon byla přepsána tak, aby byla vstřícnější a inkluzivnější. Podrobnosti viz [Nastavení e‑mailů](https://docs.pkp.sfu.ca/learning-ojs/3.4/en/settings-workflow#email-setup).

![Úprava šablon e-mailů](/images/OJS_News-in-v3-4/email_editor.png)\

Nástroje pro zadávání redakčních rozhodnutí tyto novinky využívají. V dalších verzích OJS se rozšíří i do ostatních částí systému. Více o novém procesu redakčních rozhodnutí najdete v [prezentaci](https://docs.google.com/presentation/d/e/2PACX-1vTpSVv_zY4RShrh3EfBZjHcRSYKVqDkzejDnESh6Bkg7uMgM8zFYZz-ha7j3iz_csTKump2_rI3YNWS/pub#slide=id.g16f0bb3e17f_0_26) a [videozáznamu](https://youtu.be/JEJJ1FVpao0?t=1798).

## Statistiky

Podpora standardu COUNTER byla aktualizována na [COUNTER Release 5](https://www.projectcounter.org/counter-release-5/), včetně nástrojů pro zobrazení čtenosti podle regionu a podle institucionálního přístupu. S tím přišla i základní podpora identifikátorů [ROR (Research Organization Registry)](https://ror.org/) pro institucionální předplatné.

> Viz [prezentace](https://docs.google.com/presentation/d/e/2PACX-1vTpSVv_zY4RShrh3EfBZjHcRSYKVqDkzejDnESh6Bkg7uMgM8zFYZz-ha7j3iz_csTKump2_rI3YNWS/pub#slide=id.g16f0bb3e17f_0_44) a [videozáznam](https://youtu.be/JEJJ1FVpao0?t=122).

## Trvalé identifikátory

Podpora identifikátorů DOI a služby CrossRef byla kompletně přepracována – ve spolupráci s CrossRef s cílem odstranit časté nejasnosti z předchozí verze.

> Viz [prezentace](https://docs.google.com/presentation/d/e/2PACX-1vTpSVv_zY4RShrh3EfBZjHcRSYKVqDkzejDnESh6Bkg7uMgM8zFYZz-ha7j3iz_csTKump2_rI3YNWS/pub#slide=id.g16f0bb3e17f_0_14) a [videozáznam](https://youtu.be/JEJJ1FVpao0?t=501).

## Uživatelé v multi-časopiseckých systémech

Od verze OJS 3.4.0 mohou manažeři časopisu přidávat do svého časopisu uživatelů bez ohledu na to, zda je uživatel aktivní i v jiných časopisech. Dříve bylo často nutné takové případy předávat správcům webu. ([GitHub issue #7391](https://github.com/pkp/pkp-lib/issues/7391))

## Formátování názvů příspěvků

Názvy příspěvků mohou nyní obsahovat základní formátování – tučné písmo, kurzívu, podtržení, horní a dolní index. To je využitelné zejména u článků uvádějících taxonomické názvy, které se obvykle píší kurzívou, a u recenzních článků, které mohou na recenzovaný zdroj odkazovat podtrženým názvem. ([GitHub issue #2564](https://github.com/pkp/pkp-lib/issues/2564))

## Další významné změny

- Přesun fulltextové indexace mimo proces zasílání příspěvku, což vedle ke zrychlení procesu.
- Mezi metadata lze nově zařadit i prohlášení o dostupnosti dat (data availability statement).
- Do systémových e‑mailových oznámení, která to podporují (nové číslo, oznámení, upozornění na diskusi apod.), se nově přidává přímý odkaz „Odhlásit odběr". Užiovatel tak má možnost si své e-mailové správy nastavit přímo.

## Další informace

Podrobnosti k těmto změnám najdete v prezentaci „December 2022 Development Update" od vývojařského týmu PKP – jako [prezentaci](https://docs.google.com/presentation/d/e/2PACX-1vTpSVv_zY4RShrh3EfBZjHcRSYKVqDkzejDnESh6Bkg7uMgM8zFYZz-ha7j3iz_csTKump2_rI3YNWS/pub) a [videozáznam](https://www.youtube.com/watch?v=JEJJ1FVpao0).

## O tomto překladu

Tento text vychází z originálu v dokumentaci PKP: [About Open Journal Systems (OJS) – Learning OJS 3.4](https://docs.pkp.sfu.ca/learning-ojs/3.4/en/about-ojs) (v angličtině).

Pro základní překlad do češtiny byl použit **Claude (model Claude Opus 4.8)** od společnosti Anthropic. Překlad byl následně zkontrolován, doplněn a upraven.