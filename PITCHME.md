# DALPHI

<img style="box-shadow: none; border: none; background: transparent; max-width: 75vw; max-height: 30vh;" src="img/dalphi-logo.svg" alt="Dalphi Logo" />

#### DALPHI Active Learning Platform for Human Interaction

#HSLIDE

## Motivation

- Supervised Machine Learning needs annotated data
- Existing training data are
  - often outdated
  - in military context
  - too universal or too specific
- Need to generate own training data
- Existing solutions are time consuming and exhausting
- ... and as such expensive

#HSLIDE

## Example:<br />Named Entity Recognition

- Inconvenient available annotation interfaces
- Mostly with linguistic focus
- Only whole document views
- Distribution to annotators done manually

#VSLIDE

### GATE

<img src="img/screenshots/gate.png" style="height: 40vh;" alt="GATE" />

#VSLIDE

### brat rapid annotation tool

<img src="img/screenshots/brat.png" style="height: 40vh;" alt="brat" />

#VSLIDE

### WebAnno

<img src="img/screenshots/webanno.jpg" style="height: 40vh;" alt="WebAnno" />

#HSLIDE

<ul>
  <li style="margin-bottom: 2rem;">
    To solve these problems, we restructured the way annotations are done fundamentally.
  </li>
  <li class="fragment" style="margin-bottom: 2rem;">
    We designed an iterative workflow to automate as much as we can and to save annotator's attention.
  </li>
  <li class="fragment">
    And created the OpenSource project Dalphi.
  </li>
</ul>

#HSLIDE

## Dalphi

- Web application, runs everywhere
- Helps building and maintaining annotated data
- Key features:
  - Iterating active learning supported workflow framework
  - Human readable presentation
  - Server side to propose useful annotations
  - Parallel distribution to annotators
  - Problem-agnostic document handling

#HSLIDE

## Terminology

- Service
- Raw data
- Annotation document
- Statistic
- Interface
- Project

#VSLIDE

### Service

<img src="img/architecture/service.svg" style="border: 0; padding: 20px;" alt="Service" />

- *any system* capable of communicating over HTTP
- maintaining *problem specific* jobs
- three types:
	- Iterate
	- Merge
	- Machine Learning

#VSLIDE

### Raw data

<img src="img/architecture/raw-data.svg" style="border: 0; padding: 20px;" alt="Raw data" />

- data that needs *to be annotated*

#VSLIDE

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

#VSLIDE

### Annotation document

<img src="img/architecture/annotation-document.svg" style="border: 0; padding: 20px;" alt="Annotation document" />

- a *subset* of raw data
- document which is *renderable* and *annotable*

#VSLIDE

### Statistic

<img src="img/architecture/statistic.svg" style="border: 0; padding: 20px;" alt="Statistic" />

- *key-value* pair
- mostly chronological numeric values

#VSLIDE

### Interface

<img src="img/architecture/interface.svg" style="border: 0; padding: 20px;" alt="Interface" />

- *problem specific* user interface
- renders an annotation document as a subset of raw data

#VSLIDE

### Project

<img src="img/architecture/complete.svg" style="border: 0; padding: 20px; height: 40vh;" alt="Project" />

#HSLIDE

#### Projects

<img class="screenshot" src="img/screenshots/projects.png" alt="Projects" />

#VSLIDE

#### Dashboard

<img class="screenshot" src="img/screenshots/projects-dashboard.png" alt="Projects Dashboard" />

#VSLIDE

#### Raw data

<img class="screenshot" src="img/screenshots/projects-raw-data.png" alt="Projects Raw Data" />

#VSLIDE

#### Edit raw datum

<img class="screenshot" src="img/screenshots/projects-raw-data-edit.png" alt="Projects Raw Data Edit" />

#VSLIDE

#### Annotation documents

<img class="screenshot" src="img/screenshots/projects-annotation-documents.png" alt="Projects Annotation Documents" />

#VSLIDE

#### Show annotation document

<img class="screenshot" src="img/screenshots/projects-annotation-documents-show.png" alt="Projects Annotation Documents Show" />

#VSLIDE

#### Annotators

<img class="screenshot" src="img/screenshots/projects-annotators.png" alt="Projects Annotators" />

#VSLIDE

#### Show Annotator

<img class="screenshot" src="img/screenshots/projects-annotators-show.png" alt="Projects Annotators Show" />

#VSLIDE

#### Statistics table

<img class="screenshot" src="img/screenshots/projects-statistics-table.png" alt="Projects Statistics Table" />

#VSLIDE

#### Statistics graph

<img class="screenshot" src="img/screenshots/projects-statistics-graph.png" alt="Projects Statistics Graph" />

#HSLIDE

#### Services

<img class="screenshot" src="img/screenshots/services.png" alt="Services" />

#VSLIDE

#### Edit service

<img class="screenshot" src="img/screenshots/services-edit.png" alt="Services Edit" />

#HSLIDE

#### Interfaces

<img class="screenshot" src="img/screenshots/interfaces.png" alt="Interfaces" />

#VSLIDE

#### Edit Interface

<img class="screenshot" src="img/screenshots/interfaces-edit.png" alt="Interfaces Edit" />

#VSLIDE

#### Test Interface

<img class="screenshot" src="img/screenshots/interfaces-show.png" alt="Interfaces Test" />

#HSLIDE

#### Annotators

<img class="screenshot" src="img/screenshots/annotators.png" alt="Annotators" />

#VSLIDE

#### Edit Annotator

<img class="screenshot" src="img/screenshots/annotators-edit.png" alt="Annotators Edit" />
