# La Liga-prediktor

Et sideprosjekt der jeg bruker Python og maskinlæring til å spå resultater i spanske La Liga: hjemmeseier, uavgjort eller borteseier.

Prosjektet bygger på det jeg har lært i fagene Data Collection and Analysis og AI in Cybersecurity.

## Status: under arbeid

- [x] Datainnhenting med web scraping (requests + BeautifulSoup)
- [x] Manuell datarensing i ren Python, uten pandas
- [x] Utforskende analyse og visualisering
- [x] Feature engineering: form fra de 5 siste kampene
- [x] Første modell: logistik regresjin (50,1% accuracy mot baseline 48,5%)
- [ ] KNN til sammenligning

## Data

Kampdata fra [football-data.co.uk](https://www.football-data.co.uk/spainm.php), sesongene 2015/16–2025/26 (4180 kamper). Dataen lastes ned automatisk når notebooken kjøres.

## Funn så langt

- Hjemmelaget vinner 45,7 % av kampene. Det er baselinen modellen må slå.
- Uten publikum (koronaperioden) falt andelen hjemmeseire fra 46,3 % til 41,4 %.
- Skudd på mål henger dobbelt så sterkt sammen med mål som skudd totalt (korrelasjon 0,58 mot 0,29).
- Logistikk regresjon treffer 50,1% på sesonger 2025/26, mot 48,5% for å alltid gjette hjemmeseier. Modellen gjetter nesten aldri uavgjort.
## Kjør selv

    pip install requests beautifulsoup4 pandas matplotlib scikit-learn

Åpne notebooken og kjør alle cellene.
