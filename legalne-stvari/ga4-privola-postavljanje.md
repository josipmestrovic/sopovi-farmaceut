# Kolačići i privola: kako uskladiti GA4 (interna uputa)

Ovo je interna uputa za postavljanje, nije pravni dokument i ne objavljuje se na forumu. Cilj je da stvarno stanje na forumu odgovara onome što piše u [politici privatnosti](privatnost.md#heading--kolacici).

## Zašto je ovo važno

Google Analytics 4 postavlja analitičke kolačiće. Po pravilima EU-a (GDPR + ePrivacy), analitički kolačići smiju se učitati **tek nakon što posjetitelj da privolu**. Ako se GA4 učita odmah, prije pristanka, politika privatnosti opisuje stanje koje u praksi nije usklađeno, bez obzira na to koliko je tekst dobar.

Zato GA4 treba povezati s bannerom za privolu i postaviti ga tako da se po zadanom **ne** učitava dok korisnik ne pristane.

## Što treba postaviti (3 koraka)

1. **Uključi banner za privolu na Discourseu.**
   U administraciji foruma (Admin → Postavke) potraži postavke vezane uz privolu / kolačiće i uključi prikaz bannera za privolu. Banner mora ponuditi jasan izbor: prihvati ili odbij analitičke kolačiće, bez unaprijed označenih kvačica.

2. **Postavi GA4 da se učita tek nakon pristanka.**
   Koristi **Google Consent Mode v2** sa zadanim stanjem `denied` za `analytics_storage`. Tek kad korisnik klikne "Prihvaćam", stanje se mijenja u `granted` i GA4 počinje bilježiti. Bez pristanka GA4 se ne smije učitavati niti slati podatke.

3. **Provjeri da nužni kolačići rade i bez privole.**
   Kolačići za prijavu, sesiju i sigurnost (Discourse) su nužni i smiju raditi bez privole. Banner se ne smije odnositi na njih, nego samo na analitičke kolačiće.

## Kako provjeriti da radi

Brzi test u pregledniku (alati za razvojne programere → Application → Cookies):

- **Prije** nego što klikneš išta na banneru: ne smije postojati GA kolačić (`_ga`, `_ga_*`). Smiju postojati samo Discourseovi nužni kolačići.
- Klikni **"Odbijam"**: GA kolačić se i dalje **ne** pojavljuje, forum normalno radi.
- Klikni **"Prihvaćam"**: tek tada se pojavi `_ga` i GA4 počinje bilježiti posjet.

Ako se `_ga` pojavi prije pristanka, Consent Mode nije ispravno postavljen.

## Veza s politikom privatnosti

Sekcija o kolačićima u [politici privatnosti](privatnost.md#heading--kolacici) već je napisana na način koji odgovara ovom postavu: nužni kolačići bez privole, analitički (GA4) samo uz privolu, uz mogućnost promjene odluke. Kad postaviš banner, tekst ne treba mijenjati.

## Napomena

- Google Search Console ne postavlja kolačiće za praćenje na uređaju posjetitelja, pa za njega ne treba privola.
- Ovo je tehnička uputa, ne pravni savjet. Za potpunu sigurnost (osobito jer je riječ o zdravstvenom forumu) vrijedi konzultirati stručnjaka za zaštitu podataka. Ako želiš dodatnu sigurnost, razmisli o gotovom alatu za upravljanje privolama (CMP) koji je usklađen s Google Consent Modeom.
