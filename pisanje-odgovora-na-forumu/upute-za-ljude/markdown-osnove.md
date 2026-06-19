# Markdown osnove za forum

Forum se piše u markdownu. To je jednostavan način da tekstu dodaš podebljano, liste, linkove i tablice bez ikakvih gumba, samo s par znakova. Ovdje je samo ono što ti stvarno treba za odgovor. Kako sve to izgleda složeno zajedno vidiš u [primjeru dobrog odgovora](../upute-za-agente/primjer-dobrog-odgovora.md).

## Podebljano i kurziv

Podebljano dobiješ tako da riječ omotaš s dvije zvjezdice, a kurziv s jednom.

```
ovo je **podebljano**
ovo je *kurziv*
```

Koristi ih rijetko. Naglasak djeluje samo dok ga je malo.

## Liste

Bullet listu radiš tako da svaki redak počneš crticom i razmakom.

```
- prva stavka
- druga stavka
- treća stavka
```

Numeriranu listu radiš brojevima. Nju koristi samo kad je redoslijed bitan, kao kod koraka.

```
1. prvi korak
2. drugi korak
3. treći korak
```

Ostavi prazan red prije liste, inače se zna spojiti s tekstom iznad.

## Linkovi

Link se piše tako da u uglate zagrade staviš tekst koji se vidi, a u oble zagrade adresu.

```
[članak o vitaminu D](https://farmaceut.hr/dodaci-prehrani/vitamin-d-djelovanje-i-doziranje/)
```

Tekst u zagradi neka opisuje kamo vodi. Ne lijepi goli URL i ne piši "klikni ovdje".

## Citat (za upozorenja)

Redak koji počne sa znakom > prikaže se kao izdvojeni citat. Zgodno za upozorenje.

```
> Ako se simptomi ne smire za nekoliko dana, javi se liječniku.
```

## Crta za odvajanje

Tri crtice u zasebnom redu naprave vodoravnu liniju. Njome odvajamo na primjer preporuke i izvore na dnu odgovora.

```
---
```

## Naslove ne koristimo

Znak # radi naslov, ali u odgovorima na forumu naslove ne koristimo. Umjesto njih ide kratka podebljana fraza na početku odlomka.

## Tablice

Tablicu ne moraš tipkati od nule. Uzmi gotov predložak, prepiši ga u odgovor i samo zamijeni tekst u ćelijama.

Predložak s dva stupca:

```
| Stupac A | Stupac B |
|:---|:---|
| podatak | podatak |
| podatak | podatak |
```

Predložak s tri stupca:

```
| Stupac A | Stupac B | Stupac C |
|:---|:---|:---|
| podatak | podatak | podatak |
| podatak | podatak | podatak |
```

Prvi red su nazivi stupaca. Drugi red s dvotočkama i crticama govori da je stupac poravnat lijevo, njega ne diraš. Ostali redovi su podaci.

**Kako dodati novi redak:** kopiraj jedan red podataka i zalijepi ga ispod. Svaki red mora imati isti broj okomitih crtica.

```
| Stupac A | Stupac B |
|:---|:---|
| podatak | podatak |
| podatak | podatak |
| novi red | i ovdje |
```

**Kako dodati novi stupac:** dodaj jednu okomitu crticu i ćeliju u svaki red, uključujući red s nazivima i red s dvotočkama.

```
| Stupac A | Stupac B | novi stupac |
|:---|:---|:---|
| podatak | podatak | novo |
| podatak | podatak | novo |
```

Iznad tablice stavi jednu rečenicu koja najavi što se u njoj vidi. Ispod tablice ne treba natpis.

## Česte greške

- zaboravljen prazan red prije liste ili tablice pa se sve spoji u jedan blok
- različit broj okomitih crtica po redovima pa se tablica raspadne
- goli URL umjesto opisnog teksta linka.
