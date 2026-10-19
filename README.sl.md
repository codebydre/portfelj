<p align="center">
  <img src="assets/logo.svg" alt="Portfelj" width="96">
</p>

<h1 align="center">Portfelj</h1>

<p align="center">
  Orodje za analizo portfelja in priprava davčnih napovedi za eDavke za Interactive Brokers.
</p>

<p align="center">
  <a href="README.md">English</a> · <b>Slovenščina</b>
</p>

<p align="center">
  <a href="https://portfelj.net/sl/">Spletna stran</a> ·
  <a href="https://portfelj.net/sl/get-the-app">Namestitev</a> ·
  <a href="https://github.com/codebydre/portfelj/releases">Izdaje</a> ·
  <a href="CHANGELOG.md">Dnevnik sprememb</a>
</p>

---

Portfelj iz flex poročil Interactive Brokers pripravi jasen pregled vašega portfelja in davčne napovedi, pripravljene za uvoz v eDavke. Že danes ga lahko uporabljate v terminalu, kmalu pa tudi kot namizno aplikacijo.

## Namizna aplikacija — kmalu

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/app-dark.webp">
  <img src="assets/app-light.webp" alt="Namizna aplikacija Portfelj">
</picture>

Namizna aplikacija za macOS, Windows in Linux, zgrajena na istem jedru kot orodje CLI. Prenesite flex poročila, preglejte svoje pozicije in izvozite davčne napovedi za eDavke brez uporabe terminala.

> [!TIP]
> Spremljajte ta repozitorij (**Watch → Custom → Releases**) in GitHub vas bo obvestil, ko bo aplikacija izšla.

## Orodje CLI

Na voljo že zdaj za Windows, macOS in Linux (x64 in ARM64).

```sh
# Prenos flex poročil neposredno z IBKR
portfelj flex web-service download 2026

# Pregled zaključnih poslov v letu 2026
portfelj ledger --tax-year 2026

# Priprava davčnih napovedi za eDavke
portfelj edavki --tax-year 2026
```

## Funkcionalnosti

- **Davčne napovedi za eDavke**, pripravljene iz flex poročil IBKR
- **Neposreden prenos flex poročil** z IBKR, brez ročnega izvoza
- **Korporacijska dejanja**: razcepitve in združitve delnic, prevzemi, odcepitve, spremembe izdaje, zapadlost zakladnih menic
- **Prenosi med računi** IB, vključno s selitvami med podružnicami IB
- **Prihajate od drugega borznega posrednika?** Ročno vnesite prenesene pozicije
- **Flex explorer** za iskanje vrednostnih papirjev in poslov v vaših poročilih

## Namestitev

| Platforma | Ukaz |
|---|---|
| macOS | `brew install codebydre/portfelj/portfelj` |
| Windows | Prenesite datoteko `.msi` z [Izdaj](https://github.com/codebydre/portfelj/releases) |
| Ubuntu / Debian | Prenesite datoteko `.deb` z [Izdaj](https://github.com/codebydre/portfelj/releases) in zaženite `sudo dpkg -i portfelj_*.deb` |

Podrobna navodila in preverjanje podpisa namestitvenih datotek najdete na [portfelj.net/sl/get-the-app](https://portfelj.net/sl/get-the-app).

## Dokumentacija

- [Nastavitev flex poročil](https://portfelj.net/sl/flex-reports)
- [Oddaja v eDavke](https://portfelj.net/sl/edavki)
- [Korporacijska dejanja](https://portfelj.net/sl/corporate-actions)
- [Prenosi](https://portfelj.net/sl/transfers)
- [Aktivacija aplikacije](https://portfelj.net/sl/activate)
- [Podpora](https://portfelj.net/sl/support)

## Licenca

Portfelj je lastniška programska oprema in zahteva aktivacijo. Na voljo je brez kakršnih koli jamstev. Preden se pri davčni napovedi zanesete na njegove izračune, preberite izjavo o omejitvi odgovornosti, prikazano ob prvem zagonu.
