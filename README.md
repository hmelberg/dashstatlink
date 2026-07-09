# dashstatlink

Navneregister for openstat/safestat: korte navn → script-adresser.

En hash som `safestat.no/#demo` slås opp i `names.json` her, og scriptet
kjøres som notebook/dashboard (scriptets `#options.view` avgjør visningen).

## Registrere et navn

Legg til en linje i `names.json` via commit eller pull request:

```json
{
  "mittnavn": "bruker.repo.sti.fil.py",
  "annet-navn": "https://raw.githubusercontent.com/bruker/repo/main/fil.py"
}
```

Verdien er enten kortformen `bruker.repo.sti.fil.ext` (punktum blir `/`,
main/master prøves) eller en rå URL. Navn: små bokstaver, siffer og
bindestrek, ingen punktum.
