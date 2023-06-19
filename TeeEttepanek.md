---
permalink: TeeEttepanek
---

Käsitlemata probleem või vajadus, mida MFN võiks aidata lahendada?

___Tee ettepanek___ uue nõude lisamiseks, aegunud nõude eemaldamiseks, nõude sõnastuse parandamiseks või nõuete refaktoorimiseks (ühendamiseks, lahkulöömiseks). Tee ettepanek, <a href='https://github.com/e-gov/eesti-ee-mfn/issues' target='_new'>avades issue</a> MFN-i repos, esitades _pull request_-i [MFN-i repos](https://github.com/e-gov/eesti-ee-mfn/) või saates e-kirja RIA Riigiportaali osakonna tootejuhtidele. Igaühel on õigus teha ettepanekuid nõuete lisamiseks, ümbersõnastamiseks ja ka eemaldamiseks. Ettepanekud arutatakse läbi. 

___Hea nõue___: 1) suunab tellijat ja seejärel ka arendajat; 2) ei piirdu üksiku kogemusega, vaid pakkub standardset lahendusteed sageliesinevale, tüüpilisele vajadusele või probleemile; 3) toimib ka meelespeana (et olulist asja ära ei unustataks). Nõuete lõppeesmärk on, et tekiks kasutajatele väärtust pakkuv ja turvaline tarkvara, mille arendus- ja käitluskulud on madalad; tarkvara, mida on võimalik agiilselt arendada ja mis on jätkusuutlik ka pikemas perspektiivis.

Loetavuse huvides on nõuded organiseeritud ___kategooriatesse___. Nõudel peaks olema selge, lühike, üldjuhul kindlas kõneviisis ___sõnastus___, mida kommenteerib, vajadusel ka pehmendab ___selgitus___. Nõuded nummerdatakse.

Nõudel on mõtet, kui see aitab lahendada mingit ___probleemi___ või rahuldada mingit ___vajadust___.

Vältida tuleks olukorda, kus lugeja ei saa aru, mis probleemi nõue aitab lahendada. Seetõttu lahendatav probleem vahel vajab väljaütlemist või selgitamist.

Probleemide arutamiseks on hea kasutada GitHub repo _issue_-sid. Tehniliselt kirjeldatakse nõue [MFN repo](https://github.com/e-gov/eesti-ee-mfn/) kaustas `_data` asuvas YAML-failis `Nouded.yml`. 

## Kuidas mõistet lisada?

- Mõistete kirjeldused on failis `_data\Moisted.yml`.
- Mõiste elemendid:
  - `moiste` - mõiste nimetus
  - `selgitus` - mõiste selgitus

## Kuidas nõuet lisada?

- Nõuete kirjeldused on failis `_data\Nouded.yml`.
- Nõude elemendid:
  - `name` - kategooria nimetus
  - `title` - kategooria pealkiri
  - `notes` - kategooria märkused (kuvatakse muust tekstist eristatult)
  - `requirements` - kategooria alla kuuluvad nõuded (iga nõude alla saab omakorda lisada veel selle alla kuuluvaid nõudeid)
    - `number` - nõude number
    - `name` - nõude nimetus / kirjeldus
    - `sections` - sektsioonid (nõuete grupi eristamiseks)
      - `name` - sektsiooni pealkiri
      - `requirements` - sektsiooni alla kuuluvad nõuded (iga nõude alla saab omakorda lisada veel selle alla kuuluvaid nõudeid)
        - `number` - nõude number
        - `name` - nõude nimetus / kirjeldus
- Muudatuste tegemisel tuleks täiendada ka muutelugu (failis `Muutelugu.md`):
  - muudatuse kuupäev
  - muudatuse lühikirjeldus, soovitavalt viitega vastavale nõudele.

___Vt ka___: [mittefunktsionaalsed nõuded](https://et.wikipedia.org/wiki/Mittefunktsionaalsed_n%C3%B5uded) (Vikipeedia);  Riigi Infosüsteemide Arenduskeskus (2006) [Mittefunktsionaalsete nõuete kirjeldamise juhend](https://www.ria.ee/public/publikatsioonid/Mittefunk_nouded.doc) v 0.2.
