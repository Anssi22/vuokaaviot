# Vuokaaviot
Tässä on vuokaaviot.

Vessahätä
```mermaid
graph TD;
    A([Aloitus: Kakkahätä!]) --> B([Menet kakalle!])
    B --> C{Onko paperia?}
    C -- Kyllä --> D[Pyyhi!]
    C -- Ei --> E[Käy kaupasta paperia.]
    E --> C
    D --> F[Ole iloinen ja puhdas, vedä pönttö!]
    E --> F
```
---
Lampun sytyttäminen
```mermaid
graph TD;
    subgraph NIMI
        A[Lamppu ei toimi] --> B{Lamppu kytketty?}
        B -- Kyllä --> D{Polttimo palanut?}
        D -- Ei --> F[Osta uusi lamppu]
    end
    B -- Ei --> C[Kytke lamppu]
    B -- Kyllä --> D{Polttimo palanut?}
    D -- Kyllä --> E[Vaihda polttimo]
    D -- Ei --> F[Osta uusi lamppu]
```
---
Lomapäivä
```mermaid
graph TD;
    A[aloita] --> B[katso ulos ikkunasta]
    B --> C{sataako?}
    C -- kyllä --> D[pyysy kotona]
    C -- ei --> E[mene rannalle]
    D --> F[lopeta]
    E --> F
```
---
Herätys aamulla
```mermaid
graph TD;
    A[Alku] --> B[Herätyskello soi]
    B --> C[Lepää]
    C --> D{Oletko valmis nousemaan?}
    D -- Ei --> E[Käytä Snooze-toimintoa]
    D -- Kyllä --> F[Nouse ylös sängystä]
    F --> G[Loppu]
```
---
Mikä luku
```mermaid
graph TD;
    A([Alku]) --> B[Lue luku]
    B --> C{luku == 0}
    C -- yes --> D["Luettu luku oli 0"]
    C -- no --> E["Luettu luku ei ollut 0"]
    D --> F[Loppu]
    E --> F[Loppu]
```
---
Lukupeli
```mermaid
graph TD;
    A([Alku]) --> B[Pyydä kaveria valitsemaan luku ja pitämään sen mielessä]
    B --> C[Valitse itse jokin luku]
    C --> D[Kysy kaverilta oliko valitsemasi luku sama kuin hänen]
    D --> E{Luvut olivat samat}
    E -- EI --> C[Valitse itse jokin luku]
    E -- Kyllä --> F([Loppu])
```
