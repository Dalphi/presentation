# DALPHI

<img style="box-shadow: none; border: none; background: transparent; max-width: 75vw; max-height: 40vh;" src="img/dalphi-logo.svg" alt="Dalphi Logo" />

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

## Example: Named Entity Recognition

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

- Raw data
- Annotation document
- Project
- Service
- Interface


### Raw data

- data that needs *to be annotated*

`raw-data.json`  
```
{
	"foo": "bar",
	"foobar": 1.23
}
```

`raw-data.html`  
```
<h1>Impressum</h1>
<p>3antworten UG (haftungsbeschränkt)<br>Karl-Kunger Straße 64<br>12435 Berlin</p>
```

`raw-data.jpg`  
<img src="img/cat.jpg" style="height: 15vh;" alt="Cat" />


### Annotation document

- a *subset* of raw data
- document which is *renderable* and *annotable*


### Interface

- *problem specific* user interface
- renders an annotation document as a subset of raw data


### Service

- *any system* capable of communicating over HTTP
- maintaining *problem specific* jobs
- three types:
	- Iterate
	- Merge
	- Machine Learning


### Project

...

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
