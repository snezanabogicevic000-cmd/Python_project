# Analiza hokej podataka

Mali projekat u kome sam prikupila podatke o NHL hokej timovima sa interneta i analizirala ih, kao da radim za kladionicu koja treba da odredi početne kvote za klađenje.

## Šta sam radila

1. **Preuzela podatke** sa sajta sa hokej statistikama, koristeći Selenium da otvorim stranice i sačuvam ih.
2. **Izvukla podatke** iz sačuvanih stranica pomoću BeautifulSoup-a i sačuvala ih u JSON fajl.
3. **Analizirala podatke** pomoću pandas i matplotlib - očistila ih, izračunala statistiku, napravila grafike, i pronašla neke neobične vrednosti (outliers).
4. **Predložila kvote** za klađenje na osnovu te analize, podelivši timove u grupe od najboljih do najslabijih.

## Struktura foldera

```
data/raw/         - sirovi HTML fajlovi
data/interim/      - podaci u JSON formatu
data/processed/    - finalni podaci u CSV formatu
notebooks/          - svi koraci, jedan po jedan, u Jupyter notebook-ovima
```

## Korišćeno

- Selenium
- BeautifulSoup
- pandas
- matplotlib

## Napomena

Ovo je vežba, pa su neke stvari pojednostavljene - npr. "najbolji tim" je određen samo po broju pobeda u sezoni, ne po stvarnom šampionu lige.
