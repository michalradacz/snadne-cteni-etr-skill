# Úvod

Na tomto webu najdete především technické nástroje pro podporu tvorby textů ve formě tzv. snadno čitelném textu (anglicky ETR).

Tvorba textů v tomto tvaru je částečně povinnost, ale především je to naprosto zásadní pro určité osoby, ale samotné psaní v ETR, respektive přepis normálního textu do formy ETR, je věc složitá a vyžaduje dost velké znalosti a striktní dodržování určených pravidel a mnoho praxe.

Žijeme ale v době umělé inteligence a automatizace a ETR je krásnou ukázkou toho, jak dobře připravený nástroj, může prakticky pomoci autorům textů pro jejich tvorbu či převod do ETR.

- [Používáte-li umělou inteligenci, podívejte se na tzv. skill pro tvorbu ETR](#skill-pro-ai)
- [Používáte-li pokročilé jazykové nástroje, podívejte se na šablonu se sémantickými pravidly](#pravidla-vale)
- [Hledáte-li jen metodiky a doporučení pro ETR, podívejte se do sekce s metodikami](#metodiky-etr)

# Snadné čtení

## Co je snadné čtení

Snadné čtení je způsob, jak psát texty jednoduše.
Takovým textům rozumí skoro každý.
Anglicky se snadnému čtení říká Easy to Read.
Zkráceně se mu říká ETR.

### Jak vypadá text ve snadném čtení

Text ve snadném čtení má krátké věty.
Každá věta má jen jednu myšlenku.
Každá věta začíná na novém řádku.
Text používá slova, která lidé znají.
Když je v textu těžké slovo, text ho hned vysvětlí.

Text ve snadném čtení má také:

- velké a jasné písmo
- jasné nadpisy
- hodně volného místa
- obrázky, které pomáhají textu rozumět

### Pro koho je snadné čtení

Snadné čtení je pro lidi, kterým čtení dělá potíže.
Jsou to například:

- lidé s mentálním postižením
- lidé, kteří hůř pamatují a hůř se soustředí
- lidé, kteří se teprve učí česky
- někteří starší lidé
- lidé, kteří hůř čtou

Snadné čtení pomůže i lidem v těžké situaci.
Třeba když se stala nehoda.
Člověk je pak ve stresu.
Dlouhý a složitý text mu nepomůže.

### Proč je snadné čtení důležité

Každý člověk má právo na informace.
Každý člověk má právo jim rozumět.
To říkají i úmluvy a zákony.

Když lidé textu rozumí, mohou se rozhodovat sami.
Mohou si sami vyřídit věci na úřadě.
Nemusí čekat, až jim to někdo vysvětlí.

Když lidé textu nerozumí, zůstanou stranou.
Někdo jiný pak rozhoduje za ně.

Snadné čtení pomáhá všem.
Jednoduchý text se čte rychleji.
Jednoduchému textu rozumí víc lidí.

## Kdo pravidla pro snadné čtení napsal

Pravidla napsali lidé z celé Evropy.
Pomáhali jim i lidé s mentálním postižením.
Ministerstvo vnitra podle nich napsalo pravidla pro české úřady.

## Metodiky ETR

K dispozici jsou následující:

- [MV ČR – Zvyšování srozumitelnosti materiálů veřejné správy (ETR)](https://mv.gov.cz/clanek/zvysovani-srozumitelnosti-materialu-verejne-spravy-etr.aspx)
- [MV ČR – Easy to read (ETR): metodika, vzorové texty a leták](https://kvalitavs.gov.cz/metodiky-dokumenty-a-publikace/easy-to-read-etr/)
- [MV ČR – Metodika srozumitelného a zjednodušeného vyjadřování ve veřejné správě, 2019 (PDF)](https://kvalitavs.gov.cz/modules/file_storage/download.php?file=1dabcf63%7C122&inline=1)
- [MV ČR – Leták se základními pravidly ETR (PDF)](https://kvalitavs.gov.cz/modules/file_storage/download.php?file=ae176038%7C127&inline=1)
- [Vláda ČR – Metodika Easy to read](https://www.vlada.cz/cz/ppov/vvozp/dokumenty/metodika-easy-to-read-174932/)
- [Inclusion Europe – Informace pro všechny: Evropská pravidla pro tvorbu snadno srozumitelných informací (PDF)](https://www.inclusion-europe.eu/wp-content/uploads/2017/06/CZ_Information_for_all.pdf)
- [Inclusion Europe – Evropská pravidla, kontrolní seznam a logo ETR](https://www.inclusion-europe.eu/easy-to-read-standards-guidelines/)
- [SPMP ČR – Srozumitelné informace](https://www.spmpcr.cz/co-delame/srozumitelne-informace/)
- [SPMP ČR – Publikace ve snadném čtení ke stažení](https://www.spmpcr.cz/produkty/93)
- [NZIP – Metodika snadného čtení: co to je?](https://www.nzip.cz/clanek/1528-metodika-snadneho-cteni-co-to-je)

# Skill pro AI


Zde je připravený takzvaný **skill pro umělou inteligenci** tedy připravená schopnost.

V tomto případě jde o schopnosti AI tvořit, převádět a kontrolovat texty v ETR.

## Jak skill nainstalovat?

Skill je jeden soubor `etr.skill`. Stáhnete ho odkazem níže.

- [Rovnou stáhnout etr.skill soubor](https://raw.githubusercontent.com/michalradacz/snadne-cteni-etr-skill/main/etr.skill)
- [Stránka etr.skill souboru na GitHubu](https://github.com/michalradacz/snadne-cteni-etr-skill/blob/main/etr.skill)


### Claude.ai (web, desktop, mobil)

1. Přihlaste se do [Claude.ai](https://claude.ai).
2. Otevřete **Nastavení → Capabilities** a zapněte **spouštění kódu a vytváření souborů**. Bez této funkce skill nepoběží.
3. Ve stejné části najděte **Skills** a klikněte na **Upload skill**.
4. Vyberte stažený soubor `etr.skill`.
5. Zkontrolujte, že je skill v seznamu zapnutý.

Skill je pak dostupný ve všech vašich konverzacích.

### Claude Code

Soubor `etr.skill` je obyčejný ZIP. Rozbalte ho a složku `etr` zkopírujte do adresáře se skilly:

- `~/.claude/skills/etr` pro všechny projekty,
- `.claude/skills/etr` jen pro aktuální projekt.

### ChatGPT

Skills v ChatGPT jsou zatím dostupné hlavně v pracovních účtech Business, Enterprise a Edu.

1. Stáhněte soubor `etr.skill` a přejmenujte ho na `etr.zip`.
2. V ChatGPT otevřete v postranním panelu **Skills**.
3. Klikněte na **Create** a vyberte **Upload from your computer**.
4. Vyberte soubor `etr.zip` a potvrďte instalaci.
5. Skill voláte napsáním `@etr` na začátek zprávy.

### ChatGPT bez Skills (vlastní GPT)

Tento postup funguje u osobních účtů, kde Skills nejsou.

1. Rozbalte soubor `etr.skill`. Je to obyčejný ZIP.
2. Otevřete **Explore GPTs → Create → Configure**.
3. Do pole **Instructions** napište: *Při každém požadavku se řiď přiloženým souborem SKILL.md. Jeho pravidla jsou závazná.*
4. Do **Knowledge** nahrajte soubory `SKILL.md`, `slovnik-nahrad.md`, `priklady.md` a `kontrola_etr.py`.
5. V části **Capabilities** zapněte **Code Interpreter**. Díky tomu GPT spustí i kontrolní skript.
6. GPT uložte a pojmenujte, například „Snadné čtení“.

### Gemini (Gem)

1. Rozbalte soubor `etr.skill`.
2. Otevřete [gemini.google.com](https://gemini.google.com) a v menu vyberte **Gems → Nový Gem**.
3. Do **Instrukcí** napište: *Při každém požadavku se řiď přiloženým souborem SKILL.md. Jeho pravidla jsou závazná.*
4. Do **Znalostí** nahrajte soubory `SKILL.md`, `slovnik-nahrad.md` a `priklady.md`.
5. Gem uložte a pojmenujte.

Gem nespustí kontrolní skript. Kontrolu proto dělá jen model podle kontrolního seznamu.

### Gemini CLI

V terminálu spusťte:

 gemini skills install https://github.com/michalradacz/snadne-cteni-etr-skill.git --path skills/etr

### Codex, Cursor, GitHub Copilot a další vývojářské nástroje

V terminálu spusťte:

 npx skills add michalradacz/snadne-cteni-etr-skill

Nástroj nabídne, do kterých AI nástrojů má skill nainstalovat. Místo příkazu můžete rozbalenou složku `etr` zkopírovat ručně do adresáře se skilly vašeho nástroje.

### Jiná AI

Když vaše AI skilly nepodporuje, použijte vlastní instrukce nebo projekt:

1. Rozbalte soubor `etr.skill`.
2. Vytvořte projekt nebo asistenta s vlastními instrukcemi.
3. Do instrukcí vložte obsah souboru `SKILL.md`, nebo ho přiložte jako soubor.
4. Přiložte i soubory ze složky `references`.

Bez spouštění kódu nepoběží kontrolní skript. Výsledek proto doporučujeme zkontrolovat nástrojem [Vale se stylem ETR-cs](https://github.com/michalradacz/snadne-cteni-etr-skill).



## Jak skill používat?

Nejjednodušší je napsat na začátek zprávy `/etr` a za něj text, který chcete převést. Místo textu můžete přiložit dokument (Word, PDF, webovou stránku, tabulku nebo prezentaci) a napsat jen `/etr`.

Příklady:

- `/etr Převeď tento text: …`
- `/etr` a přiložený soubor `rozhodnuti.pdf`
- `/etr Převeď přiložený leták. Čtenáři jsou senioři.`

Skill se spustí i bez příkazu, když AI požádáte o text „ve snadném čtení“, „snadno čitelný“ nebo „pro lidi s mentálním postižením“.

**Tipy pro lepší výsledek:**

- **Řekněte, pro koho text je.** Když to neuvedete, skill píše pro dospělého člověka s mentálním postižením. Takovému textu porozumí všichni ostatní.
- **Přiložte celý dokument.** Skill potřebuje vidět všechny údaje, aby žádný nevynechal.
- **Požádejte o formát.** Když chcete výsledek jako soubor Word, napište to. Jinak dostanete text přímo v chatu nebo jako soubor Markdown.
- **Upravujte v konverzaci.** Když se vám něco nelíbí, napište, co změnit. Skill úpravu znovu zkontroluje.

## Co a jak skill dělá?

Skill převádí texty do snadného čtení podle **Metodiky Easy to Read Ministerstva vnitra ČR** a **Evropských pravidel Inclusion Europe**. Všechna pravidla má v sobě, takže nic nestahuje z internetu.

Při každém převodu postupuje v sedmi krocích:

1. **Přečte celý vstup.** Umí text z chatu i dokumenty, včetně naskenovaných PDF.
2. **Rozebere obsah.** Určí čtenáře a hlavní sdělení. Sepíše si všechny povinné údaje, tedy termíny, částky, kontakty, co si čtenář má vzít s sebou a co se stane, když nic neudělá.
3. **Připraví osnovu.** Informace seřadí tak, jak je čtenář potřebuje v životě, krok za krokem.
4. **Napíše text.** Dodržuje přitom 57 závazných pravidel.
5. **Zkontroluje text strojově.** Vestavěný skript hledá dlouhé věty, zkratky, procenta, data zapsaná číslicemi, trpný rod, závorky, úřední slova a další prohřešky. Text neodevzdá, dokud skript hlásí chybu.
6. **Zkontroluje obsah.** Projde kontrolní seznam a ověří, že v textu jsou všechny povinné údaje. Ověří také, že údaje odpovídají originálu a že nic nepřidal.
7. **Předá výsledek.** Text vždy začíná větou „Toto je verze ve snadno čitelném textu.“

Pravidla, která skill dodržuje:

- věty mají nejvýš 15 slov a nesou jednu myšlenku,
- každá věta začíná na novém řádku,
- odstavec má nejvýš 5 vět,
- čtenáře oslovuje přímo „vy“,
- používá činný rod a kladné věty,
- nepoužívá zkratky, cizí slova, metafory ani procenta,
- data píše s měsícem slovy, peníze jako „500 korun“,
- těžká slova vysvětluje hned a na konci přidá slovníček,
- píše dospělým jazykem, bez dětských výrazů.

**Co skill neumí:** Nevytváří obrázky a piktogramy, které metodika doporučuje. Nevkládá evropské logo Easy to Read, které patří organizaci Inclusion Europe. Metodika také doporučuje ověřit text s lidmi, pro které je určený. U důležitých textů, jako jsou rozhodnutí úřadů nebo lhůty, proto doporučujeme výsledek aspoň jednou porovnat s originálem.
```

# Další technikálie

multisection

## ✏️Sémantická pravidla ETR

## Pravidla Vale

Vale je standard pro sémantická jazyková pravidla. Nástroje podporující tento standard umí po importu pravidel vytvářet, upravovat a korigovat text a pomáhat uživateli se správným textem respektive s dodržováním pravidel.

Ke stažení jjsou:

- [Vale pravidla pro ETR pro český jazyk](vale-etr-cs.zip)
- [ETR rules for english ETR text](vale-en.zip)


Dokumentaci k syntaxi a nástrojům najdete na https://vale.sh/docs

❗️ NNezapomeňte, že pravidla pro angličtinu a pro češtinu jsou odlišná a specifická pro jazyk, takže importujte správný balíček.

# Kontakt

Michal Rada

michal.rada@egdilna.cz

Vytvořeno v rámci úkolu Pracovního výboru Rady vlády pro osoby se zdravotním postižením

Na tvorbě spolupracovali EGdílna, Magistrát Hlavního města Prahy