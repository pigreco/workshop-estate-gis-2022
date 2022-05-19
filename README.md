# Workshop estate GIS 2022 UNIPD

---

**INDICE**

<!-- TOC -->

- [Workshop estate GIS 2022 UNIPD](#workshop-estate-gis-2022-unipd)
  - [Titolo](#titolo)
  - [Relatore](#relatore)
  - [Data, luogo e durata](#data-luogo-e-durata)
  - [Piattaforme e Software](#piattaforme-e-software)
  - [Programma](#programma)
  - [QGIS e il WMS AdE](#qgis-e-il-wms-ade)
  - [link utili](#link-utili)
  - [Contatti](#contatti)
    - [Totò Fiandaca](#totò-fiandaca)
- [Workshop WMS Catasto AdE in QGIS](#workshop-wms-catasto-ade-in-qgis)
  - [Servizio WMS](#servizio-wms)
    - [Come aggiungere il Servizio WMS a QGIS](#come-aggiungere-il-servizio-wms-a-qgis)
    - [Quali dati espone il servizio WMS](#quali-dati-espone-il-servizio-wms)
  - [Creare un nuovo GeoPackage](#creare-un-nuovo-geopackage)
  - [Impostazioni Progetto](#impostazioni-progetto)
  - [Espressione personalizzata](#espressione-personalizzata)
  - [campi virtuali](#campi-virtuali)
  - [Digitalizzazione particelle](#digitalizzazione-particelle)
    - [Plugin GIMP Selection Feature](#plugin-gimp-selection-feature)
      - [Workflow](#workflow)
    - [Plugin Magic Wand](#plugin-magic-wand)
      - [Workflow](#workflow-1)
    - [estrarre dati dai poligoni](#estrarre-dati-dai-poligoni)
    - [estrarre dati lungo linee](#estrarre-dati-lungo-linee)
- [Cosa occorre](#cosa-occorre)
  - [Software da installare](#software-da-installare)
  - [Plugin da installare](#plugin-da-installare)
- [Caratteristiche utilizzate nel progetto](#caratteristiche-utilizzate-nel-progetto)
- [Riferimenti utili](#riferimenti-utili)
- [Cosa c'è in questo repo](#cosa-cè-in-questo-repo)
- [Video demo](#video-demo)
- [Licenza](#licenza)
  - [Prossimi eventi](#prossimi-eventi)

<!-- /TOC -->

---

## Titolo

**TITOLO**: <br> Dal CAD al GIS: Mappe Catastali, disegno CAD e Tavole di Progetto.

**DESCRIZIONE**: <br> Hai mai utilizzato funzioni avanzate per utilizzare QGIS come un software CAD? Avanziamo con un flusso di lavoro che parte dallo straordinario contributo di Salvatore Fiandaca (pigrecoinfinito.com) per la gestione delle particelle catastali e avanza con l'obiettivo di condividere skills aggiundive in QGIS. Una demo per imparare a disegnare e progettare proprio come un CAD per poi proseguire con composizione di stampa avanzata.

<p align="center"><a href="https://www.mastergiscience.it/2021/05/09/estate-gis-2021/" target="_blank"><img src="./imgs//locandina/../locandine/provvisoria.jpg" width="500" title="EstateGIS2022+6"></a></p>

---

[![GitHub license](https://img.shields.io/badge/License-Creative%20Commons%20Attribution%204.0%20International-blue)](https://github.com/pigreco/seminario-estate-gis-2020/blob/master/license)
[![GitHub commit](https://img.shields.io/github/last-commit/pcm-dpc/COVID-19)](https://github.com/pigreco/seminario-estate-gis-2020/commits/master)

## Relatore

- 👨‍🦲 **Totò FIANDACA** <br>(Membro [OpenDataSicilia](http://opendatasicilia.it/) (2014) , Membro [QGIS Italia](http://qgis.it/) (2015), Socio [GFOSS.it](https://gfoss.it/) (2017), Membro [QGIS organization](https://github.com/qgis) (2020))

## Data, luogo e durata

- 🗓 29/06/2022 con orario 🕟 17:30 🕢 19:30 
- 🌐 on-line
- ⏳ 2️⃣ ore

## Piattaforme e Software

- [ZOOM](https://zoom.us/) - per diretta web
- Windows 10 64b - come SO
- [`QGIS 3.24 Tisler`](https://qgis.org/it/site/) <img src = "./imgs/qgis-icon32.png" width =15> e Plugin <img src = "./imgs/plugin_gimp.png" width =15>[`Gimp Selection feature`](https://github.com/lmotta/gimpselectionfeature_plugin/wiki) e <img src = "./imgs/plugin_magic.png" width =15>[`Magic Wand`](https://plugins.qgis.org/plugins/MagicWand-master/)
- GIMP 2.10 <img src = "./imgs/gimp_logo.png" width =15>

## Programma

1. Presentazione iniziale da parte degli organizzatori;
2. Rapida illustrazione del Workshop Estate 2021
   1. come aggiungere il WMS del catasto AdE in QGIS;
   2. come usarle il WMS come layer;
   3. quali layer sono presenti nel WMS e a quale scala sono visibili;
   4. quali SR sono disponibili nel WMS;
   5. come fare una semplice interrogare del WMS in QGIS;
   6. quali dati espone il WMS;
   7. come estrarre i dati esposti dal WMS;
   8. come creare/usare espressioni personalizzate;
   9.  come digitalizzare le particelle in modo veloce;
   10. quali plugin usare per estrarre le particelle;
3. Workshop Estate 2022
    1. Estrarre i dati catastali lungo un tracciato stradale;
    2. Modellatore grafico;
    3. Disegno CAD avanzato;
    4. Stampa tracciato e lista delle particelle;
    5. Plugin Cadastral Divisions per il frazionamento


[↑ torna su ↑](#workshop-estate-gis-2021-unipd)

## QGIS e il WMS AdE

<p align="center"><a href="https://qgis.org/it/site/" target="_blank"><img src="./imgs/WMS1.png" width="700" title="QGIS e WMS Catasto AdE in CC BY 4.0"></a></p>


[↑ torna su ↑](#workshop-estate-gis-2020-unipd)

## link utili

- **URL servizio WMS** : https://wms.cartografia.agenziaentrate.gov.it/inspire/wms/ows01.php
- **PDF su WMS** : <https://www.agenziaentrate.gov.it/portale/documents/20143/260417/Manuale+consultazione+cartografia_Documentazione+descrittiva+del+servizio+di+consultazione+della+cartografia+catastale+20180611.pdf/35e955f7-2344-56c8-1157-8f7567531660>
- **Capabilities** : <https://wms.cartografia.agenziaentrate.gov.it/inspire/wms/ows01.php?SERVICE=WMS&VERSION=1.3.0&REQUEST=GetCapabilities>
- **Pagina con URL e licenza** : https://www.agenziaentrate.gov.it/portale/web/guest/schede/fabbricatiterreni/consultazione-cartografia-catastale/servizio-consultazione-cartografia
- **espressione personalizzata**: <https://gist.github.com/pigreco/86589dddf5a59b3a7650267d5af237bd>

---

## Contatti

### Totò Fiandaca

* ✉ **Mail**: <pigrecoinfinito@gmail.com>
* **Twitter**: <https://twitter.com/totofiandaca>
* **Canale Telegram**: <https://t.me/pigrecoinfinito>

---

# Workshop WMS Catasto AdE in QGIS

## Servizio WMS

### Come aggiungere il Servizio WMS a QGIS

1. URL: `https://wms.cartografia.agenziaentrate.gov.it/inspire/wms/ows01.php`
2. Gestione delle Sorgentidati | WMS/WMTS | Nuovo :

![](imgs/wms_01.png)

<https://geoportale.cartografia.agenziaentrate.gov.it/age-inspire/srv/ita/catalog.search;jsessionid=2D812F23AA0C878D6F2DE54F9CE259CB.node1#/home>

### Quali dati espone il servizio WMS

1. codice Belfiore;
2. foglio;
3. particella;
4. sezione;
5. allegato;
6. sviluppo



## Creare un nuovo GeoPackage

- Per chi volesse avere tutto pronto, scarica geopackage con progetto (posizionato in Sicilia)

Per creare velocemente un nuovo **GeoPackage**, digitare `Ctrl+Shift+N`, altrimenti dal _Menu | Crea Vettore | Nuovo Layer GeoPackage_

<p align="center"><a href="https://qgis.org/it/site/" target="_blank"><img src="./imgs/gpkg.png" width="400" title="Nuovo Layer GeoPackage"></a></p>

1. definire il percorso e nome del GeoPackage;
2. definire il nome della tabella (`catasto`);
3. definire il Tipo di geometria (in questo esempio `Punto`);
4. selezionare EPSG del Progetto (che deve essere EPSG del WMS Catasto);
5. pigiare su `OK`

NB: il GeoPackage creerà automaticamente il campo `fid`, tutti gli altri campi che ci serviranno saranno `campi virtuali` (vedi sotto)

## Impostazioni Progetto

1. definire l'area in cui lavorare (es: un comune);
2. in funzione dell'area, definire EPSG del WMS (proiettato e non geografico);
3. installare la funzione personalizzata;
4. caricare il geopackage appena creato;
5. aggiungere il layer WMS Catasto (vedi punto 2) e selezionare i layer:
   1. Particelle;
   2. vestizione;
   3. copyright
6. occhio alla scala di visualizzazione del layer;

[↑ torna su ↑](#workshop-estate-gis-2021-unipd)

## Espressione personalizzata

Questa espressione personalizzata permette di estrarre i dati esposti dal WMS Catasto

```python
# -*- coding: utf-8 -*-
"""
/***************************************************************************
 WMS Catasto Agenzia delle Entrate CC BY 4.0
                              -------------------
        copyright            : (C) 2020 by Giulio Fattori
        email                : xxxx.xxxxx@tin.it
 ***************************************************************************/
"""

from qgis.core import *
from qgis.gui import *
import requests

@qgsfunction(args='auto', group='Custom')
def get_parcel_info2(xx, yy, EPSG, feature, parent):
    """
    <h1>WMS Catasto Agenzia delle Entrate CC BY 4.0:</h1><br>    
    La funzione, tramite una richiesta GetFeatureInfo, restituisce le informazioni utili sulla particella che ricade sotto il pixel di mio interesse:
    <h2>Esempio:</h2>
    <ul>
      <li>get_parcel_info2(355461.5,4222490.7,'EPSG:3045') -> 'IT.AGE.PLA.G273_0033A0.673'</li>
      <li>get_parcel_info2("fieldX", "fieldY",'EPSG:3045') -> 'IT.AGE.PLA.G273_0033A0.673'</li>
      <li>get_parcel_info2("fieldX", "fieldY",@project_crs) -> 'IT.AGE.PLA.G273_0033A0.673'</li>
    </ul>
    <h2>NB: le coordinate X e Y devono essere espresse nel EPSG utilizzato (gli EPSG disponibili sono:25832/3/4,3044/5/6)</h2>
    """
    req = "https://wms.cartografia.agenziaentrate.gov.it/inspire/wms/ows01.php?REQUEST=GetFeatureInfo&SERVICE=WMS&SRS="+EPSG+"&STYLES=&VERSION=1.1&FORMAT=image/png&BBOX="+str(xx-1)+","+str(yy-1)+","+str(xx+1)+","+str(yy+1)+"&HEIGHT=9&WIDTH=9&LAYERS=CP.CadastralParcel&QUERY_LAYERS=CP.CadastralParcel&INFO_FORMAT=text/html&X=5&Y=5"

    r = requests.get(req, auth=('user', 'pass'))
    a = r.text.partition("InspireId localId</th><td>")[2]
    b = a.partition("</td>")[0]
    return b
```

file da salvare nella cartella del profilo corrente: `C:\Users\nomeUtente\AppData\Roaming\QGIS\QGIS3\profiles\default\python\expressions`

raggiungibile da : Menu | Impostazioni | Profilo utente | Apri la cartella del profilo attivo

<p align="center"><a href="https://qgis.org/it/site/" target="_blank"><img src="./imgs/profilo_utente.png" width="600" title="Impostazioni | Profilo"></a></p>

la funzione personalizzata nel Gruppo Custom del field calc:

<p align="center"><a href="https://qgis.org/it/site/" target="_blank"><img src="./imgs/field_calc.png" width="600" title="Gruppo Custom - Field Calc"></a></p>

[↑ torna su ↑](#workshop-estate-gis-2021-unipd)

## campi virtuali

sotto le espressioni utilizzate nei campi virtuali (i campi virtuali permettono di creare un layer con i campi popolati da espressioni)

Creare un vettore puntuale, per esempio in un GeoPackage e definire solo il campo `fid`, gli altri campi li definiamo come `campi virtuali`, ecco le definizioni:

nome campo | tipo campo | espressione | descrizione
-----------|------------|-------------|-----------
fid | automatico | - | generato dal GeoPackage
x | virtuale | `$x` | coordinata x del punto
y |virtuale | `$y` | coordinata y del punto
catasto | virtuale | `get_parcel_info2("x","y")`| funzione personalizzata
codice | virtuale | `regexp_replace("catasto",'^(.+)\\.(.+)\\.(.+)\\.(.+)_(.+)\\.(.+)$','\\4')` | estrazione codice Belfiore
foglio | virtuale | `regexp_replace("catasto",'^(.+)\\.(.+)\\.(.+)\\.(.+)_(.+)\\.(.+)$','\\5')` | nro foglio
particella | virtuale | `regexp_replace("catasto",'^(.+)\\.(.+)\\.(.+)\\.(.+)_(.+)\\.(.+)$','\\6')` | nro particella


## Digitalizzazione particelle

### Plugin GIMP Selection Feature

- **GIMP**: <https://www.gimp.org/>
- **Plugin**: <https://plugins.qgis.org/plugins/gimpselectionfeature_plugin/> 

#### Workflow

1. Avviare QGIS e installare il Plugin GIMP Selection Feature;
2. Avviare GIMP e verificare che ci siam un menu **IBAMA**;
3. Avviare il servizio dal menu IBAMA;
4. in QGIS caricare il WMS catasto AdE e posizionarsi in un'area;
5. Avviare il plugin da **Menu Raster**;
6. Comparirà la finestra del plugin agganciata sul lato destro dello schermo;
7. nel riquadro `Visible Images` ci sarà l'elenco dei layer raster caricati nella TOC e attivi;
8. dopo aver centrato l'area da digitalizzare nella map canvas: pigiare il bottone `Send image`;
9. dopo qualche secondo, l'immagine della map canvas apparirà in GIMP;
10. usare lo _Strumento seleziona fuzzy_ e cliccare dentro una particella;
11. da QGIS, pigiare sul bottone `Get feature` per acquisire area selezionata come poligono.

Per maggiori info: <https://github.com/lmotta/gimpselectionfeature_plugin/wiki>

### Plugin Magic Wand

- <https://plugins.qgis.org/plugins/MagicWand-master/>

#### Workflow

1. Impostare _Precisione_ e _Soglia_ colore e fare clic sulla mapcanvas dove si desidera creare un poligono;
2. La modalità singola ti consente di creare UN poligono intorno a dove hai cliccato.
3. Una maggiore precisione richiede più tempo.
4. Per rendere il poligono in modo appropriato, è meglio regolare alta la Saturazione.

NB: il poligono che restituisce ha lo stesso EPSG del Progetto.

[↑ torna su ↑](#workshop-estate-gis-2021-unipd)

### estrarre dati dai poligoni

nel caso di poligoni (che hanno un EPSG diversoda quello del WMS):

```
/*estrae il foglio e la particella catastale a partire da un poligono*/
/*con EPSG diverso da quello del WMS*/

with_variable('fp',
		with_variable('geom',
				transform($geometry,'EPSG:4326', @project_crs ),
				get_parcel_info2(
						x( point_on_surface( @geom)),
						y( point_on_surface( @geom)), @project_crs)),
	regexp_replace( @fp ,'^(.+)\\.(.+)\\.(.+)\\.(.+)_(.+)\\.(.+)$', '\\5/\\6')
		    	)
```

```
/*estrae il foglio e la particella catastale a partire da un poligono*/
/*con EPSG uguale a quello del WMS*/

with_variable('fp',
get_parcel_info2(
x( point_on_surface($geometry)),
y( point_on_surface($geometry)),@project_crs),
regexp_replace(@fp ,'^(.+)\\.(.+)\\.(.+)\\.(.+)_(.+)\\.(.+)$', '\\5/\\6')
			)
```

### estrarre dati lungo linee

```
........
```

[↑ torna su ↑](#workshop-estate-gis-2021-unipd)

# Cosa occorre

Software con caratteristiche minime per seguire con profitto il workshop

## Software da installare

1. [QGIS 3.24 Tisler](https://qgis.org/it/site/) (o maggiore) <img src = "./imgs/qgis-icon32.png" width =15>;
2. [GIMP 2.10](https://www.gimp.org/) (attualmente GIMP 2.10.24) <img src = "./imgs/gimp_logo.png" width =15>;

##  Plugin da installare

1. [GIMP Selection Feature](https://plugins.qgis.org/plugins/gimpselectionfeature_plugin/) <img src = "./imgs/plugin_gimp.png" width =15>;
2. [Magic Wand](https://plugins.qgis.org/plugins/MagicWand-master/) <img src = "./imgs/plugin_magic.png" width =15>;
3. [Nominatim Locator Filter](https://plugins.qgis.org/plugins/nominatim_locator_filter/) <img src = "https://raw.githubusercontent.com/rduivenvoorde/nominatim_locator_filter/master/icons/icon.svg" width =15>
4. [Cadastral Divisions](https://github.com/Korto19/Cadastral_Divisions)

[↑ torna su ↑](#workshop-estate-gis-2021-unipd)

# Caratteristiche utilizzate nel progetto

1. servizio WMS;
2. Geopackage;
3. espressioni personalizzate e non;
4. espressioni regolari;
5. campi virtuali;
6. Plugin;
7. GIMP;
8. Etichette con funzione custom.
9. Decorazioni: Copyright, Immagine, Etichetta Titolo;
10. Modellatore grafico;
11. Strumenti di disegno CAD avanzato;
12. Compositore di Stampe
13. Plugin Frazionamenti.

[↑ torna su ↑](#workshop-estate-gis-2021-unipd)

# Riferimenti utili

- **WorkShop EstateGIS 2021** : <https://github.com/pigreco/workshop-estate-gis-2021>
- **QGIS** : <https://qgis.org/it/site/>
- **Repo QGIS** : <https://github.com/qgis/QGIS/blob/master/README.md>
- **Plugin Gimp Selection Feature** : <https://plugins.qgis.org/plugins/gimpselectionfeature_plugin/>
- **Plugin Magic Wand** : <https://plugins.qgis.org/plugins/MagicWand-master/>
- **Plugin Cadastral Divisions** : <https://github.com/Korto19/Cadastral_Divisions>
- **Nominatim Locator Filter** : <https://plugins.qgis.org/plugins/nominatim_locator_filter/>
- **Consultazione cartografia catastale - WMS** : <https://www.agenziaentrate.gov.it/portale/web/guest/schede/fabbricatiterreni/consultazione-cartografia-catastale/servizio-consultazione-cartografia>
- **GIMP** : <https://www.gimp.org/>
- **Font Trueno** : <https://www.wfonts.com/font/trueno>
- **Visual Style Guide** : <https://www.qgis.org/en/site/getinvolved/styleguide.html#trueno-fonts>
- **Visual Studio Code** : <https://code.visualstudio.com/>
- **onData** : <https://ondata.it/>
- **OpenDataSicilia** : <http://opendatasicilia.it/>
- **Blog Post di Andrea Borruso** : <https://medium.com/tantotanto/le-mappa-castali-diventano-finalmente-utilizzabili-821db2f84533>

[↑ torna su ↑](#workshop-estate-gis-2021-unipd)

# Cosa c'è in questo repo

- cartella `imgs` contiene le immagini utilizzate nel progetto .qgs;
- cartella `risorse` contiene i file utilizzati nel progetto, come:
  - geopackage [particelle_WMS.gpkg](https://github.com/pigreco/workshop-estate-gis-2021/raw/main/risorse/particelle_WMS.gpkg);
  - il geopackage contiene due tabelle: la prima si chiama `catasto` la seconda `particelle`;
  - il geopackage contine anche il progetto (`catasto_wms`) che fa uso della tabella `catasto`; la tabella `particella` è vuota, pronta all'uso;
- file `license` è il file che definisce la licenza del repository;
- file `README.md` è questo file, con le info.

[↑ torna su ↑](#workshop-estate-gis-2021-unipd)

# Video demo

Video 1 | Video 2 | Video 3 | Video 4
--------|---------|---------|--------
[![add_col_area_perimetro](https://img.youtube.com/vi/Fu-i0zfxndY/0.jpg)](https://youtu.be/Fu-i0zfxndY "Estrarre i dati con il Field Calc di QGIS usando un Punto") | [![add_col_area_perimetro](https://img.youtube.com/vi/ujLGbsreqYY/0.jpg)](https://youtu.be/ujLGbsreqYY "Estrarre i dati catastali a partire da un Poligono") |[![add_col_area_perimetro](https://img.youtube.com/vi/GhJwzl8HDs8/0.jpg)](https://youtu.be/GhJwzl8HDs8 "Vettorializzare particelle con il Plugin GIMP Selection Feature") | [![add_col_area_perimetro](https://img.youtube.com/vi/DBRHYJOtqFo/0.jpg)](https://youtu.be/DBRHYJOtqFo "Vettotializzare Particelle con il Plugin Magic Wand")

# Licenza

**CC BY 4.0** - <https://creativecommons.org/licenses/by/4.0/deed.it>

[↑ torna su ↑](#workshop-estate-gis-2021-unipd)

## Prossimi eventi

![](imgs/locandine/programma.png)
