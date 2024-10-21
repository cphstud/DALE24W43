Opgaver
================
2024-10-21

## Opvarmning

### Lav en testdf 20x4 dataframe på følgende måde:

- A indeholder tilfældige heltal mellem 10 og 100
- B indeholder en streng som begynder med stort bogstav, derpå 3
  karakterer som skal indeholde en vokal et mellemrum, et decimaltal på
  2 decimaler mellem 1 og 10 og derpå strengen “Dollars.” Løs dette vha
  en funktion som kan skabe de 10 strenge
- C indeholder tilfældige heltal mellem 10 og 100
- D indeholder én af tre gyldige danske postnumre

### Lav en dataframe vha tidy af frekvensen på postnumre og sorter med hyppigst forekommende øverst

### Lav et bar plot vha ggplot

### Lav et Danmarkskort hvor zip-koden farves vha hyppighed <https://github.com/sebastianbarfort/mapDK>.

### Grupper på zip og beregn mean og sd på zip vha mutate (ikke summarise)

### Subset testdf

- a så den kun består af dem hvor A er større end 80 og C under 15
- b så den kun består af dem hvor A er mindre end 60 og eller større end
  90 og begynder med en vokal

### Lav en kategorivariabel som deler A nogenlunde lige i tre grupper

# Nye boliger - vha tidyverse

### Indlæs filen <https://efif.sharepoint.com/:u:/s/cph/Lyngby/EaPp3giEjAVOvyI9LPX-az8BU-6LQfikPn52Mf1hMnZgOw?e=TIEWr1>

- 1 lav en kolonne med postnumre ud fra “addr” (brug str_extract)
  - a Lav en dataframe med de 10 hyppigst forekommende postnumre
  - b Lav et DK-plot hvor man kan se de 10 hyppigst forekommende
    postnumre
- 2 lav en kolonne med postdistrikternes navne ud fra “addr”
  - 1 lav først en kolonne med alt efter postnummeret og til slut
  - 2 fjern derpå det du ikke skal bruge
- 3 lav to kolonner med hhv vejnavn og vejnr fra addr
  - 1 lav først en basiskolonne vha str_remove
  - 2 Brug nu str_match med groups (!) til at hente tekst ud (hint:
    str_match(vejtot,“^(.\*)-\d”)\[,2\])
  - 3 Hent vejnummeret ud vha en lookbehind: (?\<=-)
- 4 lav kolonner for kvm,grund,emærke og pris
  - a Undersøg NA forekomster og vurder om de er tilfældige eller
    skyldes data?
- 5 Forbered en præsentation af datasættet baseret på ovenstående
  undersøgelse og data-science-modellen
  - a Dokumenter vigtig kode
  - b Dokumenter datasættet
    - 1 Variabel typer, relevante basisplot, outliers samt
      relations-plot (pris ~ Emærke etc)
