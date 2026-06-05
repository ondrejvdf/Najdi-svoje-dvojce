# Vyhledávač podobnosti profilu

Jednoduchá webová stránka pro zadání základních údajů, nahrání fotografie a zobrazení výsledku podobnosti profilu.

## Jak stránku spustit

1. Otevři soubor `index.html` v prohlížeči.
2. Vyplň jméno, příjmení, věk a město.
3. Nahraj fotografii přes pole `Fotka`.
4. Klikni na tlačítko `Hledat dvojce`.
5. Po dokončení analýzy se zobrazí výsledek se shodou.

## Co musí být ve složce

Struktura složky má vypadat takto:

```text
outputs/
  index.html
  README.md
  assets/
    match-1.png
    match-2.png
    match-3.png
```

## Obrázky výsledků

Výsledkové obrázky musí být uložené ve složce `assets`.

Použité názvy:

```text
assets/match-1.png
assets/match-2.png
assets/match-3.png
```

Stránka umí načíst i jiné formáty, pokud mají stejný název:

```text
match-1.jpg
match-1.jpeg
match-1.webp
```

Nejjednodušší je ale nechat soubory jako PNG:

```text
match-1.png
match-2.png
match-3.png
```

## Když se obrázek nezobrazuje

Zkontroluj:

1. Obrázky jsou opravdu ve složce `outputs/assets`.
2. Názvy souborů jsou přesně `match-1.png`, `match-2.png`, `match-3.png`.
3. V názvu není mezera navíc nebo jiné číslo.
4. Po změně souborů obnov stránku v prohlížeči přes `Ctrl + F5`.

## Úprava textů

Všechny texty jsou přímo v souboru `index.html`.

Nejdůležitější části:

```text
const funnyMatches
const scanSteps
```

V `funnyMatches` jsou nastavené výsledkové obrázky, nadpisy, popisy a procenta shody.

V `scanSteps` jsou texty, které se ukazují během progress baru.
