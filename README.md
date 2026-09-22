# etr – převod textu do snadného čtení

Skill pro Claude, který převede libovolný text nebo dokument do češtiny ve formátu
**snadného čtení** (Easy to Read, ETR).

🌐 **Web projektu:** [www.michalrada.cz/snadne-cteni-etr-skill](https://www.michalrada.cz/snadne-cteni-etr-skill)
📦 **Repozitář:** [github.com/egdilna/snadne-cteni-etr-skill](https://github.com/egdilna/snadne-cteni-etr-skill)

Výstup je určený lidem, kteří mají potíže i se srozumitelným textem. Patří k nim lidé
s mentálním postižením, lidé s demencí, cizinci se slabší češtinou, někteří senioři
a lidé ve vypjaté životní situaci.

Skill vychází z **Metodiky Easy to Read Ministerstva vnitra ČR (2019)** a z **Evropských
pravidel pro tvorbu snadno srozumitelných informací** (Inclusion Europe). Všechna pravidla
má v sobě, takže nic nestahuje a nic nevyhledává na webu.

## Co skill umí

- Převede text vložený do chatu nebo nahraný dokument (DOCX, PDF včetně skenů, HTML,
  TXT, MD, XLSX, PPTX).
- Každý výstup začne větou **„Toto je verze ve snadno čitelném textu.“**
- Zachová všechny údaje, podle kterých čtenář jedná: termíny, částky, kontakty,
  co si má vzít s sebou a co se stane, když nic neudělá.
- Nepřidává fakta, která v originálu nejsou.
- Výsledek sám zkontroluje skriptem a kontrolním seznamem. Předá ho až ve chvíli,
  kdy kontrola nehlásí žádnou chybu.
- Krátký výsledek vrátí přímo v chatu. Delší výsledek uloží jako `.md`, nebo jako `.docx`
  s typografií podle metodiky (bezpatkové písmo 14 bodů, zarovnání vlevo, bez dělení slov).

## Struktura repozitáře

```
etr/
├── SKILL.md                    # postup v 7 krocích a 57 závazných pravidel
├── references/
│   ├── slovnik-nahrad.md       # náhrady úředních a cizích slov
│   └── priklady.md             # vzorové převody „před → po“
└── scripts/
    └── kontrola_etr.py         # automatická kontrola výstupu
```

## Instalace

### Claude.ai

1. Stáhněte soubor `etr.skill` z [Releases](../../releases), nebo si složku `etr/`
   zabalte do ZIP.
2. Otevřete v Claude **Nastavení → Capabilities → Skills**.
3. Skill nahrajte.

### Claude Code

Zkopírujte složku `etr/` do adresáře se skilly:

```bash
# pro všechny projekty
cp -r etr ~/.claude/skills/

# jen pro aktuální projekt
cp -r etr .claude/skills/
```

## Použití

Skill zavoláte příkazem:

```
/etr
```

Za příkaz vložte text, nebo nahrajte dokument. Příklady:

```
/etr Převeď tento text do snadného čtení: …
/etr (a přiložený soubor rozhodnuti.pdf)
```

Skill se spustí i bez příkazu, když požádáte o text „ve snadném čtení“,
„snadno čitelný“ nebo „pro lidi s mentálním postižením“.

## Kontrolní skript

Skript funguje i samostatně, bez Claude. Potřebuje jen Python 3 a nemá žádné další závislosti.

```bash
python3 etr/scripts/kontrola_etr.py text.md
python3 etr/scripts/kontrola_etr.py text.md --json
```

Hlásí dva typy nálezů:

- **CHYBA** znamená porušení pravidla, které se musí opravit.
- **VAROVÁNÍ** znamená podezření, které je potřeba posoudit.

Kontroluje tyto věci:

- povinnou úvodní větu,
- délku věty (nejvýš 15 slov) a odstavce (nejvýš 5 vět),
- jednu větu na řádek,
- zkratky, procenta, římské číslice a data zapsaná číslicemi (15. 11. 2026),
- závorky, středníky, kurzívu, poznámky pod čarou a vnořené odrážky,
- trpný rod, zápory, souvětí, dlouhá slova, úřední slova a dlouhé internetové adresy.

Návratový kód je `0`, když text nemá chyby, a `1`, když chyby má. Skript tak jde použít
i v CI.

## Zdroje

Závazné:

- **Ministerstvo vnitra ČR:** [Metodika srozumitelného a zjednodušeného vyjadřování ve veřejné správě (Easy to Read), 2019](https://kvalitavs.gov.cz/metodiky-dokumenty-a-publikace/easy-to-read-etr/)
- **Inclusion Europe / SPMP ČR:** [Informace pro všechny – Evropská pravidla pro tvorbu snadno srozumitelných informací](https://www.inclusion-europe.eu/wp-content/uploads/2017/06/CZ_Information_for_all.pdf)

Doplňkové:

- [Leták se základními pravidly ETR (MV ČR)](https://kvalitavs.gov.cz/modules/file_storage/download.php?file=ae176038%7C127&inline=1)
- [SPMP ČR – Srozumitelné informace](https://www.spmpcr.cz/co-delame/srozumitelne-informace/)
- [NZIP – Metodika snadného čtení a příklady článků](https://www.nzip.cz/clanek/1528-metodika-snadneho-cteni-co-to-je)

## Omezení

- Skill píše jen česky.
- Obrázky a piktogramy nevytváří. Metodika je doporučuje, takže je případně doplňte ručně.
- Evropské logo Easy to Read do výstupu nevkládá. Logo patří Inclusion Europe. Smíte ho
  použít jen na text, který pravidla splňuje, a musíte k němu připojit tuto větu:
  *© European Easy-to-Read Logo: Inclusion Europe. More information at
  www.inclusion-europe.eu/easy-to-read*
- Metodika doporučuje ověřit text s lidmi z cílové skupiny. U textů s právními dopady,
  jako jsou rozhodnutí nebo lhůty, doporučujeme aspoň jednou porovnat údaje s originálem.

## Licence

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.cs) – dílo smíte sdílet a upravovat
i komerčně, pokud uvedete autora.

## Autor

Michal Rada ([EGdílna](https://github.com/egdilna)) · [web projektu](https://www.michalrada.cz/snadne-cteni-etr-skill)
