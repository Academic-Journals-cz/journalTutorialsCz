# Similarity Check v OJS

## Similarity Check
Služba **Similarity Check** je poskytována organizací *Crossref* na platformě **iThenticate** od společnosti *Turnitin*. Služba je poskytována na základě splnění podmínek poskytování služby a následném podpisu smlouvy. Redakcím odborných časopisu napomáhá nástroj s odhalováním potenciálních plagiátů a posouzením originality zaslaných rukopisů. Porovnáním textu s rozsáhlou databází publikovaného obsahu získají rychlou zpětnou vazbu o míře podobnosti s již existující literaturou. Jedná se o placenou službu, kde jsou účtovány roční poplatky společností Crossref a zároveň také poplatky za zkontrolované dokumenty. Ptejte se svého vydavatele, jak je nastavená politika financování této služby.

Více informací (v EN): [Crossref Similarity Check](https://www.crossref.org/services/similarity-check/)

Aktuálně je v rámci služby **Similarity Check** využívána nejnovější verze systému **iThenticate 2**. iThenticate je celosvětově uznávaný antiplagiátorský systém. Tento systém porovnává zaslané dokumenty s rozsáhlou databází miliard webových stránek, odborných článků, časopisů, knih a dalších publikovaných materiálů, včetně obsahu uloženého v databázích *Crossref* a *Turnitin*.

Výstupem kontroly je tzv. **Similarity Report**, který zobrazuje míru shody textu s již publikovaným obsahem a identifikuje konkrétní zdroje, se kterými se text překrývá. **Similarity Report** poskytuje editorům podklad pro odborné posouzení originality textu.

Návod, jak číst Similarity Report (v EN):
[The Similarity Report](https://guides.ithenticate.com/hc/en-us/articles/27244924185357-The-Similarity-Report)

### Struktura Similarity Report

Similarity report je standardně rozdělen do tří hlavních částí (viz obrázky níže):

**1. Informační panel**

Horní část rozhraní obsahuje základní informace o kontrolovaném dokumentu, jako je název souboru, datum kontroly, počet slov a hlavně **Similarity Score**. Jedná se o procentuální vyjádření míry shody zaslaného rukopisu s již existujícím publikovaným obsahem v databázích systému iThenticate. Detaily ohledně dokumentu je možné si zobrazit po kliknutí na ikonu **ⓘ Details**. 

![Horní panel](/images/OJS_Similarity-check/similarity_check_top_part.png)
*Obr. 1. Horní panel*

![Detaily souboru](/images/OJS_Similarity-check/filedetails_in_similarity_check.png)

*Obr. 2. Detaily souboru*


**2. Levý panel – text dokumentu**

Levý panel zobrazuje plný text kontrolovaného dokumentu. Pasáže, u kterých byla nalezena shoda s jinými zdroji, jsou barevně zvýrazněny. Orientace mezi jednotlivými zdroji v textu je zajištěna barevným rozlišením a je velmi intuitivní.

**3. Pravý panel – seznam zdrojů shody**

Pravý panel obsahuje seznam zdrojů, se kterými byl dokument porovnán a kde byla zjištěna podobnost textu. U každého zdroje je uvedena procentuální míra shody a odkazy na konkrétní části textu. Zdroje jsou seřazeny podle velikosti shody od nejvyšší po nejnižší.

![Spodní část](/images/OJS_Similarity-check/similarity_check_bottom_part.png)
*Obr. 3. Spodní část*

**Poznámka**

Pomocí funkce *Sources: Show overlapping sources* je možné si zobrazit všechny překrývající se zdroje. Výchozí nastavení je zobrazení hlavního zdroje, se kterým se text překrývá. V případě, že je stejná část textu publikovaná na více platformách, zobrazí se pouze jednaa pomocí tohoto nastavení je možnéí zobrazit všechny ostatní platformy.

### Nastavení v prostředí iThenticate

Následující nastavení předpokládá, že již máte zřízený účet v systému **iThenticate 2** prostřednictvím služby **Similarity Check** a máte oprávnění provádět kontroly podobnosti. Účty Similarity Check jsou standardně vázány na vydavatele (publisher). Pokud jste redakce časopisu, obraťte se na svého vydavatele, který vám pomůže se zřízením přístupu a přiřazením účtu.

Tento návod vychází z předpokladu, že uživatelský účet má oprávnění **"Product admin"**, které umožňuje spravovat integrace a generovat přístupové údaje pro propojení s redakčním systémem OJS.

**Integrations**
- Nejprve je nutné nastavit tzv. **Integrations**, ve kterých budou vytvořeny *TCA Scope* a *API Key* potřebné pro zajištění propojení systému **iThenticate** s OJS.
- V této sekci naleznete přehled všech vytvořených propojení, včetně seznamu klíčů (API Keys) přiřazených ke konkrétním integracím. Přehled umožňuje správu jednotlivých přístupů a kontrolu jejich platnosti.

![Seznam propojení](/images/OJS_Similarity-check/similarity_check_integrations.png)
*Obr. 4. Seznam propojení*

**TCA Scope**
- Doporučenou praxí je vytvářet samostatný *TCA Scope* pro každý časopis zvlášť. Tento postup umožňuje přehledné sledování statistik Similarity Check pro jednotlivé časopisy v prostředí OJS, zejména pokud se jedná o instalaci typu **multi-journal**.
- Pro vytvoření nového *TCA Scope* použijte tlačítko **Generate TCA Scope**.

![Generuj TCA Scope](/images/OJS_Similarity-check/similarity_check_generate_API_Scope_button.png)
*Obr. 5. Generuj TCA Scope*

- Následně zadejte název pro nově vytvářený *API Scope*. Doporučuje se použít jednoznačný a snadno identifikovatelný název, například podle názvu časopisu nebo instalace OJS.

![Generování API Scope](/images/OJS_Similarity-check/similarity_check_generate_API_Scope.png)
*Obr. 6. Generování API Scope*

**API Key**
- První klíč (*API Key*) je vytvořen během procesu generování *TCA Scope*. Název klíče je vhodné zvolit tak, aby bylo možné jej později snadno identifikovat v seznamu přístupů (např. podle názvu časopisu nebo účelu použití).

![Generovat API Key](/images/OJS_Similarity-check/similarity_check_generate_API_Key.png)
*Obr. 7. Generovat API Key*

- **Upozornění:** Vygenerovaný klíč se zobrazí pouze jednou. Po potvrzení již není možné jeho hodnotu znovu zobrazit. Doporučuje se klíč ihned bezpečně uložit, například do správce hesel nebo interní dokumentace.

![API Key vytvořen](/images/OJS_Similarity-check/similarity_check_generate_API_Key_created.png)
*Obr. 8. API Key vytvořen*

- Pro jeden *TCA Scope* je možné vytvořit libovolné množství klíčů. To může být užitečné například v případě ztráty původního klíče nebo při potřebě propojit jeden časopis s více systémy či prostředími.
- Další klíč lze v seznamu propojení vytvořit pomocí odkazu **Create New Key**.

### Nastavení v prostředí OJS

**Instalace pluginu**
- Plugin je dostupný v *Galerii pluginů* pod názvem **iThenticate** a lze jej nainstalovat přímo z administrace OJS.

![Plugin iThenticate](/images/OJS_Similarity-check/plugin_ithenticate.png)
*Obr. 9. Plugin iThenticate*

- Instalaci z galerie provedete pomocí tlačítka **Instalovat**.

![Instalace pluginu](/images/OJS_Similarity-check/plugin_ithenticate_installation.png)
*Obr. 10. Instalace pluginu*

- Zdrojový kód pluginu je dostupný také na GitHubu: https://github.com/pkp/plagiarism

- Plugin je možné využívat jak prostřednictvím služby **Similarity Check**, tak i samostatně na základě přímé smlouvy se službou **iThenticate** (Turnitin).

- Po instalaci je nutné plugin aktivovat a správně nakonfigurovat.

---

**Nastavení pluginu**
- V nastavení pluginu je potřeba vyplnit adresu API služby iThenticate a klientský **API Key**, který byl vytvořen v předchozích krocích v prostředí iThenticate (viz část **Integrations**).  
- Pro službu **Similarity Check** bude konfigurace typicky vypadat následovně:

![Nastavení pluginu](/images/OJS_Similarity-check/ithenticate_settings_01.png)
*Obr. 11. Nastavení pluginu*

- Ve výchozím nastavení jsou do iThenticate odesílány všechny soubory připojené k manuskriptu. Alternativně je možné zvolit manuální režim odesílání pouze vybraných souborů, který poskytuje větší kontrolu nad tím, které verze dokumentu budou analyzovány.

- Ostatní parametry pluginu jsou volitelné a lze je přizpůsobit podle redakčního workflow.

---

**Manuální využívání kontroly plagiátů**
- Níže je popsán postup manuální kontroly podobnosti. Pokud je aktivováno automatické odesílání, je krok nahrání souboru přeskočen a manuskript je do iThenticate odeslán automaticky po jeho odeslání autorem do redakčního řízení.

- V manuálním režimu je nutné mezi jednotlivými kroky krátce vyčkat na dokončení zpracování požadavku. Pokud je další krok spuštěn příliš brzy, může systém vrátit chybu, že předchozí operace ještě nebyla dokončena. V průběhu workflow budete vždy vyzváni k potvrzení jednotlivých akcí.

---

*1. Provést kontrolu plagiátorství / Conduct Plagiarism Check*
- Spustí nahrávání souboru do systému iThenticate.

![Provést kontrolu plagiátorství](/images/OJS_Similarity-check/similarity_check_conduct_plagiarism_check.png)
*Obr. 12. Provést kontrolu plagiátorství*

- **Upozornění:** V metadatech manuskriptu musí být v seznamu přispěvatelů nastaven *primární kontakt* (Primary Contact). Bez této informace nebude možné soubor do iThenticate odeslat.

![Nastavení primárního kontaktu](/images/OJS_Similarity-check/set_primary_contact.png)
*Obr. 13. Nastavení primárního kontaktu*

---

*2. Plánování hlášení o plagiátorství / Schedule Plagiarism Report*
- Spustí vytvoření Similarity Report v systému iThenticate.

---

*3. Obnovit skóre podobnosti plagiátů / Refresh Plagiarism Similarity Score*
- Načte aktuální procentuální hodnotu podobnosti z iThenticate a zobrazí ji v prostředí OJS.

---

*4. Zobrazení reportu v iThenticate*

![iThenticate skóre](/images/OJS_Similarity-check/ithenticate_score.png)
*Obr. 14. iThenticate skóre*

- Ikona iThenticate zároveň slouží jako přímý odkaz do **Similarity Report**, kde je možné detailně zobrazit shody textu a identifikované zdroje. Struktura reportu je popsána výše v části **Similarity Report**.
