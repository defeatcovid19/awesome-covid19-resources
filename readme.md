# awesome-covid19-resources [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of awesome resources related to COVID19.


## Contents

- [Datasets and models](#datasets-and-models)
  - [Medical Imaging](#medical-imaging)
  - [Outbreak dynamics](#outbreak-dynamics)
    - [Case datasets](#case-datasets)
    - [Government pages](#government-pages)
    - [Dashboards](#dashboards)
    - [Statistical models](#statistical-models)
- [Contribute](#contribute)
- [License](#license)



## Datasets and models

Datasets and machine learning models related to COVID-19.


### Medical Imaging

- Kaggle Dataset: Pneumonia
  https://www.kaggle.com/search?q=pneumonia+in%3Adatasets


### Outbreak dynamics

Collection of case datasets for analyzing the dynamics of the outbreak.

#### Case datasets

<table>
<tr><th>Publisher</th><th>Scope</th><th>Granularity</th><th>Updated</th><th>Fields<sup>1</sup></th><th>Format</th><th>Dataset</th></tr>
<tr><td colspan="7"><b>International level</b></td></tr>
<tr><td><a href="https://coronavirus.jhu.edu">Johns Hopkins CSSE</a></td><td>worldwide</td><td>countries<sup>2</sup></td><td>daily</td><td>1, 2, 3</td><td>csv</td><td><a href="https://github.com/CSSEGISandData/COVID-19">link</a></td></tr>
<tr><td><a href="https://www.ecdc.europa.eu/en/geographical-distribution-2019-ncov-cases">European Centre for Disease Prevention and Control</a></td><td>worldwide</td><td>countries</td><td>daily</td><td>1, 3</td><td>xls</td><td><a href="https://www.ecdc.europa.eu/en/publications-data/download-todays-data-geographic-distribution-covid-19-cases-worldwide">link</a></td></tr>
<tr><td colspan="7"><b>Country level</b></td></tr>
<tr><td><a href="http://www.protezionecivile.it/risk-activities/health-risk/emergencies/coronavirus">Protezione Civile</a></td><td>Italy</td><td><b>n</b>ational, <b>r</b>egional, <b>p</b>rovinces</td><td>daily</td><td><b>n</b>, <b>r</b>: 1, 2, 3, 4, 5, 6, 7; <b>p</b>: 1</td><td>csv, json</td><td><a href="https://github.com/pcm-dpc/COVID-19">link</a></td></tr>
</table>

<sup>[1]</sup> Fields explanation:
1. Positive cases
2. Recovered cases
3. Deaths
4. Hospitalized patients
5. Patients in intensive care unit
6. Cases in home confinement
7. COVID-19 tests made

<sup>[2]</sup> provinces for China, US, Canada, Australia


#### Government pages

Official pages for monitoring the national outbreaks with reported cases. English version is provided, if found.

**America**
- [United States](https://www.cdc.gov/coronavirus/2019-ncov/cases-updates/cases-in-us.html)

**Asia**
- [Singapore](https://www.gov.sg/article/covid-19-cases-in-singapore)

**Europe**
- [Austria](www.sozialministerium.at/coronavirus) (in German)
- [Belgium](https://www.info-coronavirus.be/en/news/)
- [Denmark](https://www.ssi.dk/aktuelt/sygdomsudbrud/coronavirus/covid-19-i-danmark-epidemiologisk-overvaagningsrapport) (in Danish)
- [Finland](https://thl.fi/en/web/infectious-diseases/what-s-new/coronavirus-covid-19-latest-updates)
- [France](https://www.santepubliquefrance.fr/maladies-et-traumatismes/maladies-et-infections-respiratoires/infection-a-coronavirus/articles/infection-au-nouveau-coronavirus-sars-cov-2-covid-19-france-et-monde) (in French)
- [Germany](https://www.rki.de/DE/Content/InfAZ/N/Neuartiges_Coronavirus/Fallzahlen.html) (in German, see [this page](https://www.rki.de/DE/Content/InfAZ/N/Neuartiges_Coronavirus/Situationsberichte/Gesamt.html) for situation reports in English)
- [Hungary](http://abouthungary.hu/news-in-brief/coronavirus-heres-the-latest/)
- [Ireland](https://www.gov.ie/en/news/7e0924-latest-updates-on-covid-19-coronavirus/)
- [Italy](http://www.salute.gov.it/portale/nuovocoronavirus/dettaglioContenutiNuovoCoronavirus.jsp?id=5351&area=nuovoCoronavirus&menu=vuoto) (in Italian)
- [Netherlands](https://www.rivm.nl/en/news/current-information-about-novel-coronavirus-covid-19)
- [Norway](https://www.fhi.no/en/id/infectious-diseases/coronavirus/dags--og-ukerapporter/daily-reports-COVID19/)
- [Portugal](https://covid19.min-saude.pt/relatorio-de-situacao/) (in Portuguese)
- [Spain](https://www.mscbs.gob.es/en/profesionales/saludPublica/ccayes/alertasActual/nCov-China/situacionActual.htm) (in Spanish)
- [Sweden](https://www.folkhalsomyndigheten.se/smittskydd-beredskap/utbrott/aktuella-utbrott/covid-19/aktuellt-epidemiologiskt-lage/) (in Swedish)
- [Switzerland](https://www.bag.admin.ch/bag/en/home/krankheiten/ausbrueche-epidemien-pandemien/aktuelle-ausbrueche-epidemien/novel-cov/situation-schweiz-und-international.html)
- [United Kingdom](https://www.gov.uk/guidance/coronavirus-covid-19-information-for-the-public#number-of-cases)


#### Dashboards

Dashboards visualizing the dynamics of the outbreak in different geographic areas.

**Worldwide**
- [Johns Hopkins University](https://gisanddata.maps.arcgis.com/apps/opsdashboard/index.html#/bda7594740fd40299423467b48e9ecf6)
- [WHO](https://experience.arcgis.com/experience/685d0ace521648f8a5beeeee1b9125cd)
- [Worldometer](https://www.worldometers.info/coronavirus/)

**Country level**
- [Italy](http://opendatadpc.maps.arcgis.com/apps/opsdashboard/index.html#/b0c68bce2cce478eaac82fe38d4138b1) - Official dashboard for monitoring the COVID-19 outbreak in Italy, provided by [Civil Protection](http://www.protezionecivile.it) of Italy
- [Portugal](https://esriportugal.maps.arcgis.com/apps/opsdashboard/index.html#/acf023da9a0b4f9dbb2332c13f635829) - Official dashboard for monitoring the COVID-19 outbreak in Portugal, provided by the [Public Health Department](https://www.dgs.pt) of Portugal
- [Singapore](https://co.vid19.sg/dashboard) - Unoffical but extremly extensive dashboard for monitoring the COVID-19 outbreak in Singapore at case-level, provided by [@zp_uca](https://twitter.com/zp_uca)
- [Spain](https://covid19.isciii.es) - Official dashboard for monitoring the COVID-19 outbreak in Spain, provided by the [Instituto de Salud Carlos III](https://www.isciii.es)


#### Statistical models

- [COVID-19 Dashboards](https://covid19dashboards.com) - Extensive collection of dashboards, diagrams and other visualizations as well as statistical models of the COVID-19 outbreak.


## Contribute

Contributions welcome! Read the [contribution guidelines](contributing.md) first.



## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0)

To the extent possible under law, Neosperience has waived all copyright and related or neighboring rights to this work.
