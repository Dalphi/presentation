# DALPHI

<img style="box-shadow: none; border: none; background: transparent; max-width: 75vw; max-height: 30vh;" src="img/dalphi-logo.svg" alt="Dalphi Logo" />

#### DALPHI Active Learning Platform for Human Interaction

---

## Motivation

- Supervised Machine Learning needs annotated data
- Dalphi helps building and maintaining annotated data
- Key features:
  - Human readable presentation
  - Parallel distribution to annotators
  - Problem-agnostic document handling

---

### Example
## Named Entity Recognition

- Inconvenient available annotation interfaces
- Mostly with linguistic focus
- Only whole document views
- No active server side to propose useful annotations
- Distribution to annotators done manually


### GATE

<img src="img/screenshots/gate.png" style="height: 40vh;" alt="GATE" />


### brat rapid annotation tool

<img src="img/screenshots/brat.png" style="height: 40vh;" alt="brat" />


### WebAnno

<img src="img/screenshots/webanno.jpg" style="height: 40vh;" alt="WebAnno" />

---

## Terminology

- Service
- Raw data
- Annotation document
- Statistic
- Interface
- Project


### Service

<img src="img/architecture/service.svg" style="border: 0; padding: 20px;" alt="Service" />

- *any system* capable of communicating over HTTP
- maintaining *problem specific* jobs
- three types:
	- Iterate
	- Merge
	- Machine Learning


### Raw data

<img src="img/architecture/raw-data.svg" style="border: 0; padding: 20px;" alt="Raw data" />

- data that needs *to be annotated*


### Raw data

`JSON`  
```
{
	"foo": "bar",
	"foobar": 1.23
}
```

`HTML`  
```
<h1>Impressum</h1>
<p>3antworten UG (haftungsbeschränkt)<br>Karl-Kunger Straße 64<br>12435 Berlin</p>
```

`JPG`  
<img src="img/cat.jpg" style="height: 15vh;" alt="Cat" />


### Annotation document

<img src="img/architecture/annotation-document.svg" style="border: 0; padding: 20px;" alt="Annotation document" />

- a *subset* of raw data
- document which is *renderable* and *annotable*


### Statistic

<img src="img/architecture/statistic.svg" style="border: 0; padding: 20px;" alt="Statistic" />

- *key-value* pair
- mostly chronological numeric values


### Interface

<img src="img/architecture/interface.svg" style="border: 0; padding: 20px;" alt="Interface" />

- *problem specific* user interface
- renders an annotation document as a subset of raw data


### Project

<img src="img/architecture/complete.svg" style="border: 0; padding: 20px; height: 40vh;" alt="Project" />


---

## Dalphi

- Ruby on Rails application

---

#### Projects

<img class="screenshot" src="img/screenshots/projects.png" alt="Projects" />


#### Dashboard

<img class="screenshot" src="img/screenshots/projects-dashboard.png" alt="Projects Dashboard" />


#### Raw data

<img class="screenshot" src="img/screenshots/projects-raw-data.png" alt="Projects Raw Data" />


#### Edit raw datum

<img class="screenshot" src="img/screenshots/projects-raw-data-edit.png" alt="Projects Raw Data Edit" />


#### Annotation documents

<img class="screenshot" src="img/screenshots/projects-annotation-documents.png" alt="Projects Annotation Documents" />


#### Show annotation document

<img class="screenshot" src="img/screenshots/projects-annotation-documents-show.png" alt="Projects Annotation Documents Show" />


#### Statistics table

<img class="screenshot" src="img/screenshots/projects-statistics-table.png" alt="Projects Statistics Table" />


#### Statistics graph

<img class="screenshot" src="img/screenshots/projects-statistics-graph.png" alt="Projects Statistics Graph" />

---

#### Services

<img class="screenshot" src="img/screenshots/services.png" alt="Services" />


#### Edit service

<img class="screenshot" src="img/screenshots/services-edit.png" alt="Services Edit" />

---

#### Interfaces

<img class="screenshot" src="img/screenshots/interfaces.png" alt="Interfaces" />


#### Edit Interface

<img class="screenshot" src="img/screenshots/interfaces-edit.png" alt="Interfaces Edit" />


#### Test Interface

<img class="screenshot" src="img/screenshots/interfaces-show.png" alt="Interfaces Test" />
