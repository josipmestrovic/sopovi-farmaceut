# Prompt: pisanje odgovora na forumu farmaceut.hr

Ovo je ulazna uputa za agenta koji piše **nove odgovore** na pitanja s foruma `forum.farmaceut.hr`. Popuni sekciju **Input** na dnu i pošalji agentu cijeli ovaj fajl. Agent prema [pravila-za-pisanje-odgovora.md](pravila-za-pisanje-odgovora.md) i uzorku iz [primjer-dobrog-odgovora.md](primjer-dobrog-odgovora.md) izrađuje gotov odgovor.


## Tijek rada

1. Pročitaj pitanje korisnika i sav priloženi materijal iz sekcije Input.
2. Napiši nov odgovor farmaceuta prema svim pravilima iz pravila-za-pisanje-odgovora.md.
3. Uskladi formu s referentnim uzorkom iz primjer-dobrog-odgovora.md.
4. U CTA blok stavljaj **samo** interne linkove koje je korisnik dao u Inputu. Ne pretražuj bazu linkova i ne izmišljaj interne URL-ove.
5. Za blok izvora koristi vanjske izvore iz Inputa. Ako ih nema ili su nedostatni, smiješ predložiti provjerene vanjske izvore iz svog znanja i označiti ih s "(provjeriti)".
6. Isporuči gotov odgovor kao markdown.

## Output

Gotov odgovor ispiši kao čisti markdown unutar code blocka (` ```markdown ... ``` `), spreman za copy-paste na forum. 

---

## Input

**Pitanje s foruma (doslovno):**

<!-- Zalijepi originalni tekst korisnika koji pita. Ne mijenja se. -->


**Interni linkovi (farmaceut.hr i forum.farmaceut.hr):**

<!-- Linkovi za CTA blok, po mogućnosti s prijedlogom anchora. -->
-


**Vanjski izvori (opcionalno):**

<!-- Provjereni izvori za blok na dnu. Ako je prazno, agent smije predložiti i označiti "(provjeriti)". -->
-


**Kontekst teme:**

<!-- Je li ovo prvi odgovor u temi ili nastavak postojeće rasprave? Ako je nastavak, zalijepi relevantne prethodne odgovore. -->


**Rod farmaceuta:** ženski 


**Dodatne napomene (opcionalno):**

<!-- Sve ostalo što agent treba znati: naglasci, doze, podpitanja za prioritet, čega se kloniti. -->
