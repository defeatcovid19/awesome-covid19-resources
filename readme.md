# awesome-covid19-resources [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of awesome resources related to COVID19.


## Contents

- [Datasets and models](#datasets-and-models)
  - [Medical imaging](#medical-imaging)
    - [Imaging datasets](#imaging-datasets)
    - [Medical imaging models](#medical-imaging-models)
  - [Epidemic data and models](#epidemic-data-and-models)
    - [Case datasets](#case-datasets)
    - [Government pages](#government-pages)
    - [Dashboards](#dashboards)
    - [Statistical models](#statistical-models)
- [Selected scientific articles](#selected-scientific-articles)
  - [Medical imaging papers](#medical-imaging-papers)
  - [Epidemic papers](#epidemic-papers)
  - [Clinical record analysis](#clinical-record-analysis)
  - [Computational drug research](#computational-drug-research)
- [Contribute](#contribute)
- [License](#license)



## Datasets and models

Datasets and machine learning models related to COVID-19.


### Medical imaging

- [Pneumonia related Kaggle Datasets](https://www.kaggle.com/search?q=pneumonia+in%3Adatasets) - A collection of medical imaging (chest X-ray or CT) datasets and other resources.

- [Coronavirus disease 2019 (COVID-19)](https://radiopaedia.org/articles/coronavirus-disease-2019-covid-19-1) article on [Radiopaedia](https://radiopaedia.org)
- [Italian RX scans of COVID-19 cases](https://www.sirm.org/category/senza-categoria/covid-19/)
#### Imaging datasets

| Name | Publisher | Type | Images | Classes |
|------|-----------|:----:|-------:|---------|
| [Chest X-Ray Images (Pneumonia)](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia) (children) | [Paul Mooney](https://www.kaggle.com/paultimothymooney) | Chest x-ray | 5,863 | Pneumonia / Normal |
| [COVID-19 image data collection](https://github.com/ieee8023/covid-chestxray-dataset) | [Joseph Paul Cohen](https://josephpcohen.com/) | Chest x-ray / CT | 158 | COVID-19, SARS, Viral Pneumonia, etc. |
| [NIH Clinical Center chest x-ray datasets](https://nihcc.app.box.com/v/ChestXray-NIHCC) | [National Institutes of Health](https://www.nih.gov/news-events/news-releases/nih-clinical-center-provides-one-largest-publicly-available-chest-x-ray-datasets-scientific-community) | Chest x-ray | 100,000+ | 14 categories including Pneumonia and Infiltration |
| [COVID19 High quality images](https://www.kaggle.com/theroyakash/covid19) | [theroyakash](https://www.kaggle.com/theroyakash) | Chest x-ray | 338 | COVID-19, Viral Pneumonia / Normal

#### Medical imaging models

Articles, blog posts describing a proposed model:
- [COVID-19 Detection Neural Network (COVNet)](https://github.com/bkong999/COVNet)
- [Detecting COVID-19 in X-ray images with Keras, TensorFlow, and Deep Learning](https://www.pyimagesearch.com/2020/03/16/detecting-covid-19-in-x-ray-images-with-keras-tensorflow-and-deep-learning/)
  - [COVID-10 detection in X-ray images using deep learning and Grad-CAM visualisation](https://www.linkedin.com/posts/sohaiblaraba_covid19-covid19-interpretability-activity-6645675878485409795-Y6gM/) - Derived work on the interpretability of the results.
  - [Deep Learning for Medical Imaging: COVID-19 Detection](https://blogs.mathworks.com/deep-learning/2020/03/18/deep-learning-for-medical-imaging-covid-19-detection/) - Ported the above model to MATLAB.
- [Using Deep Learning to detect Pneumonia caused by NCOV-19 from X-Ray Images](https://towardsdatascience.com/using-deep-learning-to-detect-ncov-19-from-x-ray-images-1a89701d1acd)



### Epidemic data and models

Collection of case datasets for analyzing the dynamics of the outbreak.

#### Case datasets

<table>
<tr><th>Scope</th><th>Publisher</th><th>Granularity</th><th>Updated</th><th>Fields<sup>1</sup></th><th>Format</th><th>Dataset</th></tr>

<tr><td colspan="7"><i>International level</i></td></tr>
<tr><td>worldwide</td><td><a href="https://coronavirus.jhu.edu">Johns Hopkins CSSE</a></td><td>countries<sup>2</sup></td><td>daily</td><td>1, 2, 3</td><td>csv</td><td><a href="https://github.com/CSSEGISandData/COVID-19">link</a></td></tr>
<tr><td>worldwide</td><td><a href="https://www.ecdc.europa.eu/en/geographical-distribution-2019-ncov-cases">European Centre for Disease Prevention and Control</a></td><td>countries</td><td>daily</td><td>1, 3</td><td>xls</td><td><a href="https://www.ecdc.europa.eu/en/publications-data/download-todays-data-geographic-distribution-covid-19-cases-worldwide">link</a></td></tr>

<tr><td colspan="7"><i>Country level</i></td></tr>
<tr><td>Canada</td><td><a href="https://github.com/ishaberry/Covid19Canada">COVID-19 Canada Open Data Working Group</a></td><td>provinces</td><td>daily</td><td>1, 2, 3, 7</td><td>Google Sheets</td><td><a href="https://github.com/ishaberry/Covid19Canada">link</a></td></tr>
<tr><td>Italy</td><td><a href="http://www.protezionecivile.it/attivita-rischi/rischio-sanitario/emergenze/coronavirus">Protezione Civile</a></td><td><b>n</b>ational, <b>r</b>egional, <b>p</b>rovinces</td><td>daily</td><td><b>n</b>, <b>r</b>: 1, 2, 3, 4, 5, 6, 7; <b>p</b>: 1</td><td>csv, json</td><td><a href="https://github.com/pcm-dpc/COVID-19">link</a></td></tr>
<tr><td>United States</td><td><a href="https://covidtracking.com/about-team/">The COVID Tracking Project</a></td><td>states</td><td>daily</td><td>1, 3, 7</td><td>Google Sheets, csv, json, GraphQL</td><td><a href="https://covidtracking.com">link</a></td></tr>
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

*Americas*
- [Canada](https://www.canada.ca/en/public-health/services/diseases/2019-novel-coronavirus-infection.html)
- [Mexico](https://coronavirus.gob.mx/noticias/)
- [United States](https://www.cdc.gov/coronavirus/2019-ncov/cases-updates/cases-in-us.html)

*Asia*
- [Isreal](https://www.health.gov.il/English/Topics/Diseases/corona/Pages/press-release.aspx)
- [Singapore](https://www.gov.sg/article/covid-19-cases-in-singapore)

*Australia and Oceania*
- [Australia](https://www.health.gov.au/news/health-alerts/novel-coronavirus-2019-ncov-health-alert/coronavirus-covid-19-current-situation-and-case-numbers)
- [New Zealand](https://www.health.govt.nz/our-work/diseases-and-conditions/covid-19-novel-coronavirus/covid-19-current-cases)

*Europe*
- [Austria](https://www.sozialministerium.at/coronavirus) (in German)
- [Belgium](https://www.info-coronavirus.be/en/news/)
- [Denmark](https://www.ssi.dk/aktuelt/sygdomsudbrud/coronavirus/covid-19-i-danmark-epidemiologisk-overvaagningsrapport) (in Danish)
- [Estonia](https://www.terviseamet.ee/en)
- [Finland](https://thl.fi/en/web/infectious-diseases/what-s-new/coronavirus-covid-19-latest-updates)
- [France](https://www.santepubliquefrance.fr/maladies-et-traumatismes/maladies-et-infections-respiratoires/infection-a-coronavirus/articles/infection-au-nouveau-coronavirus-sars-cov-2-covid-19-france-et-monde) (in French)
- [Germany](https://www.rki.de/DE/Content/InfAZ/N/Neuartiges_Coronavirus/Fallzahlen.html) (in German, see [this page](https://www.rki.de/DE/Content/InfAZ/N/Neuartiges_Coronavirus/Situationsberichte/Gesamt.html) for situation reports in English)
- [Hungary](http://abouthungary.hu/news-in-brief/coronavirus-heres-the-latest/)
- [Ireland](https://www.gov.ie/en/news/7e0924-latest-updates-on-covid-19-coronavirus/)
- [Italy](http://www.salute.gov.it/portale/nuovocoronavirus/dettaglioContenutiNuovoCoronavirus.jsp?id=5351&area=nuovoCoronavirus&menu=vuoto) (in Italian)
- [Netherlands](https://www.rivm.nl/en/news/current-information-about-novel-coronavirus-covid-19)
- [Norway](https://www.fhi.no/en/id/infectious-diseases/coronavirus/dags--og-ukerapporter/daily-reports-COVID19/)
- [Poland](https://www.gov.pl/web/koronawirus/wykaz-zarazen-koronawirusem-sars-cov-2) (in Polish)
- [Portugal](https://covid19.min-saude.pt/relatorio-de-situacao/) (in Portuguese)
- [Spain](https://www.mscbs.gob.es/en/profesionales/saludPublica/ccayes/alertasActual/nCov-China/situacionActual.htm) (in Spanish)
- [Sweden](https://www.folkhalsomyndigheten.se/smittskydd-beredskap/utbrott/aktuella-utbrott/covid-19/aktuellt-epidemiologiskt-lage/) (in Swedish)
- [Switzerland](https://www.bag.admin.ch/bag/en/home/krankheiten/ausbrueche-epidemien-pandemien/aktuelle-ausbrueche-epidemien/novel-cov/situation-schweiz-und-international.html)
- [United Kingdom](https://www.gov.uk/guidance/coronavirus-covid-19-information-for-the-public#number-of-cases)


#### Dashboards

Dashboards visualizing the dynamics of the outbreak in different geographic areas.

*Worldwide*
- [Johns Hopkins University](https://gisanddata.maps.arcgis.com/apps/opsdashboard/index.html#/bda7594740fd40299423467b48e9ecf6)
- [WHO](https://experience.arcgis.com/experience/685d0ace521648f8a5beeeee1b9125cd)
- [Worldometer](https://www.worldometers.info/coronavirus/)

*Country level*
- [Canada](https://art-bd.shinyapps.io/covid19canada/) - Case level dashboard about the COVID-19 outbreak in Canada, curated by [COVID-19 Canada Open Data Working Group](https://github.com/ishaberry/Covid19Canada)
- [Isreal](https://imoh.maps.arcgis.com/apps/webappviewer/index.html?id=20ded58639ff4d47a2e2e36af464c36e&locale=he&/) - Government dashboard for monitoring the COVID-19 outbreak in Israel (in Hebrew)
- [Italy](http://opendatadpc.maps.arcgis.com/apps/opsdashboard/index.html#/b0c68bce2cce478eaac82fe38d4138b1) - Official dashboard for monitoring the COVID-19 outbreak in Italy, provided by [Civil Protection](http://www.protezionecivile.it) of Italy
- [Portugal](https://esriportugal.maps.arcgis.com/apps/opsdashboard/index.html#/acf023da9a0b4f9dbb2332c13f635829) - Official dashboard for monitoring the COVID-19 outbreak in Portugal, provided by the [Public Health Department](https://www.dgs.pt) of Portugal
- [Singapore](https://co.vid19.sg/dashboard) - Unoffical but extremly extensive dashboard for monitoring the COVID-19 outbreak in Singapore at case-level, provided by [@zp_uca](https://twitter.com/zp_uca)
- [Spain](https://covid19.isciii.es) - Official dashboard for monitoring the COVID-19 outbreak in Spain, provided by the [Instituto de Salud Carlos III](https://www.isciii.es)


#### Statistical models

- [COVID-19 Dashboards](https://covid19dashboards.com) - Extensive collection of dashboards, diagrams and other visualizations as well as statistical models of the COVID-19 outbreak.
- [COVID-19 Health System Capacity](https://github.com/daveluo/covid19-healthsystemcapacity) - Open geospatial work to support healthcare systems' capacity in the United States.
- [Epidemic calculator](http://gabgoh.github.io/COVID/index.html) - An interactive visual calculator demonstrating the relations between different epidemic variables.


## Selected scientific articles

A collection of scientific papers related to COVID-19 relevant from the data science point of view.

- [COVID-19 Open Research Dataset](https://pages.semanticscholar.org/coronavirus-research) - A free resource of over 29,000 scholarly articles about COVID-19 and the coronavirus family of viruses
  - [Call to action](https://www.whitehouse.gov/briefings-statements/call-action-tech-community-new-machine-readable-covid-19-dataset/) of the US government on this dataset
  - [Kaggle challenge](https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge) associated with the dataset


### Medical imaging papers

*Computer Tomography (CT) images*
- [Artificial Intelligence Distinguishes COVID-19 from Community Acquired Pneumonia on Chest CT](https://pubs.rsna.org/doi/10.1148/radiol.2020200905)
- [Lung Infection Quantification of COVID-19 in CT Images with Deep Learning](https://arxiv.org/abs/2003.04655v2)
- [Rapid AI Development Cycle for the Coronavirus (COVID-19) Pandemic](https://arxiv.org/abs/2003.05037v1): Initial Results for Automated Detection & Patient Monitoring using Deep Learning CT Image Analysis
- [Deep Learning System to Screen Coronavirus Disease 2019 Pneumonia](https://arxiv.org/ftp/arxiv/papers/2002/2002.09334.pdf)
- [A deep learning algorithm using CT images to screen for Corona Virus Disease (COVID-19)](https://www.medrxiv.org/content/10.1101/2020.02.14.20023028v3)
- [Coronavirus Disease 2019 (COVID-19): A Perspective from China](https://pubs.rsna.org/doi/10.1148/radiol.2020200490) - A study discussing the use of different diagnosis tools (CT, x-ray) for early detection of COVID-19


### Epidemic papers

- [A Poisson Autoregressive Model to Understand COVID-19 Contagion Dynamics](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3551626)
- [Relationship between the ABO Blood Group and the COVID-19 Susceptibility](https://www.medrxiv.org/content/10.1101/2020.03.11.20031096v1)


### Clinical record analysis

- [Prediction of criticality in patients with severe Covid-19 infection using three clinical features](https://www.medrxiv.org/content/10.1101/2020.02.27.20028027v2): a machine learning-based prognostic model with clinical data in Wuhan
- [Abnormal respiratory patterns classifier may contribute to large-scale screening of people infected with COVID-19 in an accurate and unobtrusive manner](https://arxiv.org/abs/2002.05534v1)


### Computational drug research

- [Repurposing Therapeutics for COVID-19](https://chemrxiv.org/articles/Repurposing_Therapeutics_for_the_Wuhan_Coronavirus_nCov-2019_Supercomputer-Based_Docking_to_the_Viral_S_Protein_and_Human_ACE2_Interface/11871402/4): Supercomputer-Based Docking to the SARS-CoV-2 Viral Spike Protein and Viral Spike Protein-Human ACE2 Interface



## Contribute

Contributions welcome! Read the [contribution guidelines](contributing.md) first.



## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, Neosperience and other contributors have waived all copyright and related or neighboring rights to this work.
