# Eesti.ee mittefunktsionaalsed nõuded (MFN)

# Kuidas mõistet lisada?

- Mõistete kirjeldused on failis `_data\Moisted.yml`.
- Mõiste elemendid:
  - `moiste` - mõiste nimetus
  - `selgitus` - mõiste selgitus


# Kuidas nõuet lisada?

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
