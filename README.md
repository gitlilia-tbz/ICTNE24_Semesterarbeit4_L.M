# README

# 🏋️‍♀️ FitTracker Pro - Kubernetes Version. Tracke. Wachse. Gewinne.
![alt text](image-4.png)

### Fitness Tracking Platform - Migriert auf Kubernetes

![Project Status](https://img.shields.io/badge/Status-Active-brightgreen)![Version](https://img.shields.io/badge/Version-v1.0-blue)
![Python](https://img.shields.io/badge/Python-3.9-blue?logo=python&logoColor=white)![Top Language](https://img.shields.io/github/languages/top/gitlilia-tbz/ICTNE24_Semesterarbeit3_L.M)
![Flask](https://img.shields.io/badge/Flask-2.3.3-black?logo=flask&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-15-blue?logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-Containerized-blue?logo=docker&logoColor=white)
![AWS EC2](https://img.shields.io/badge/Deployed%20on-AWS%20EC2-orange?logo=amazon-aws&logoColor=white)
![CI/CD](https://img.shields.io/badge/CI%2FCD-GitHub%20Actions-green?logo=github&logoColor=white)
![Weather API](https://img.shields.io/badge/Weather-OpenWeatherMap-blue?logo=openweathermap&logoColor=white)

---

**Studierende:** Lilia Mechani | **Semester:** 4 | **Dozenten:** (PRJ) Corrado Parisi (CNC) Philip Stark.

[🚀 Live Demo](http://52.202.224.208/) • [📖 Repo](https://github.com/gitlilia-tbz/ICTNE24_Semesterarbeit3_L.M) • [🏗️ KanBan](https://semesterarbeit3liliam.atlassian.net/jira/software/projects/KAN/boards/1)

# Live Update:
|ArgoCD Setup: In Progress /// Aktualisierung Jira-Board: In Progress|

## Inhaltsverzeichnis

## 📋 Projektübersicht

### [1. 📊 Projektmanagement](#1--projektmanagement)

* [1.1 Projektbeschreibung](#11-projektbeschreibung)
* [1.2 Zeitplan](#12-zeitplan)
* [1.3 Risiko-Evaluation](#13-risiko-evaluation)
* [1.4 Risiko-Matrix](#14-risiko-matrix)
* [1.5 SWOT-Analyse](#15-swot-analyse)
* [1.6 Sprint-Dokumentation](#16-sprint-dokumentation)
  * [1.6.1 Sprint 1](#161-sprint-1)
  * [1.6.2 Sprint 2](#162-sprint-2)
  * [1.6.3 Sprint 3](#163-sprint-3)

* [1.7 Projekt Gantt-Diagramm](#18-projekt-gantt-diagramm)

### [2. 🛠️ Technische Dokumentation](#2-️-technische-dokumentation)

* [2.1 Architektur-Übersicht](#21-architektur-übersicht)

### [3. ☁️ Deployment](#3-️-deployment--devops)

* [3.1 AWS EC2 Setup](#31-aws-ec2-setup)
* [3.2 Kubernetes Setup](#32-kubernetes-setup)
* [3.3 ArgoCD](#33-ArgoCD)
* [3.4 YAML Files](#34-yaml-files)
* [3.5 Produktionsumgebung](#35-produktionsumgebung)

### [4. 📱 User Interface](#4--user-interface)

* [4.1 Frontend Design](#41-frontend-design)
* [4.2 User Experience](#42-user-experience)

### [5. 🧪 Testing & Qualitätssicherung](#5--testing--qualitätssicherung)

* [5.1 User-Testing](#52-user-testing)
* [5.2  10 Testfälle](#53-10-testfälle)

### [6. 📈 Ergebnisse & Reflexion](#6--ergebnisse--reflexion)

* [6.1 Erreichte Ziele](#61-erreichte-ziele)
* [6.2 Herausforderungen](#62-herausforderungen)
* [6.3 Lessons Learned](#63-lessons-learned)
* [6.4 Ausblick](#64-ausblick)

### [7. 📚 Anhang](#7--anhang)

* [7.1 Code-Repository](#71-code-repository)
* [7.2 Verwendete Technologien](#72-verwendete-technologien)
* [7.3 Quellen](#73-quellen)
* [7.4 Glossar](#74-glossar)
* [7.5 Kontaktangaben](#75-kontaktangaben)

---

# 1. 📊 Projektmanagement

## 1.1 Projektbeschreibung

Meine Microservices aus meiner letzten Semesterarbeit «TrackMyGym, Fitness Tracker PRO» werden nun in eine skalierbare Kubernetes-Umgebung übertragen. Weiterhin Cloud-Basiert und mit DevOps Pipelines deployable.
Zielsetzung der Semesterarbeit
Welche, z.B. als Aufstellung, Ziele sollen mit der Semesterarbeit erreicht werden.
Es sollten mindestens drei messbare Ziele aufgeführt werden.
1.  Die TrackMyGym Applikation bekommt ein neues Kleid. Die Microservices werden ins Kubernetes übertragen
2. Die Microservices werden innerhalb eines Skalierbaren Kubernetes Cluster betrieben. Diese wird in einer AWS EC2 Instanz gehostet. Bei erhöhter last, werden mehr Kubernetes Pods hochgefahren.
3. Eine CI/CD Pipeline wird innerhalb von GitHub Actions erstellt damit ein erfolgreiches Deployment des Images sowie Änderungen in der Code-Base nach Kubernetes erfolgen.


Die App soll auf folgenden Technologien basieren:

Werkzeuge:
-	Kubernetes -> Skalierbarkeit
-	GitHub -> Repo und Versionierung
-	Docker -> Image
-	VSCode + GitHub Add-in -> Source Code Editor und Dokumentation
-	Claude AI und Claude Code -> KI Unterstützte Entwicklung
-	Laptop -> Meine eigene Workstation

Durch die Migration zu Kubernetes wird die Applikation noch hochverfügbarer und somit Zukunftssicherer für eine breitere User-Adoption.

| :checkered_flag: Angezielte Kernfunktionen der neuen Infrastruktur                              |
| ------------------------------------------------------------------------------------------- |
| Folgende Ziele wurden gesetzt: |

1.  Die TrackMyGym Applikation bekommt ein neues Kleid. Die Microservices werden ins Kubernetes übertragen
2. Die Microservices werden innerhalb eines Skalierbaren Kubernetes Cluster betrieben. Diese wird in einer AWS EC2 Instanz gehostet. Bei erhöhter last, werden mehr Kubernetes Pods hochgefahren.
3. Eine CI/CD Pipeline wird innerhalb von GitHub Actions erstellt damit ein erfolgreiches Deployment des Images sowie Änderungen in der Code-Base nach Kubernetes erfolgen.




## 1.2 Zeitplan

Projektzeitleiste und Meilensteine
 
![alt text](image-2.png)

## 1.3 Risiko-Evaluation
Identifizierte Projektrisiken und deren Bewertung.

```mermaid
graph TB
    subgraph "Risiko Evaluation"
        subgraph Row1[" "]
            direction LR
            subgraph Hoch["🔴 HOHE AUSWIRKUNG"]
                H1["Cluster-Fehlkonfiguration"]
                H2["Fehlerhafte Architektur"]
                H3["Technische Schulden"]
                H4["API Gateway Kommunikation"]
                H5["Secrets-Verwaltung"]
            end
            subgraph Mittel1["🟡 MITTLERE AUSWIRKUNG Teil 1"]
                M1["Performance-Overhead durch K8s"]
                M2["Dokumentation unvollständig"]
                M3["Learning Curve"]
                M4["Deployment-Fehler Pipeline"]
                M5["Monitoring-Lücken"]
            end
        end
        subgraph Row2[" "]
            direction LR
            subgraph Mittel2["🟡 MITTLERE AUSWIRKUNG Teil 2"]
                M6["Service-Integration Probleme"]
                M7["Ressourcen-Limits falsch gesetzt"]
                M8["AWS-Kosten Überschreitung"]
                M9["Datenverlust bei Neustart"]
                M10["Sprint-Zeitplan Verzug"]
            end
            subgraph Niedrig["🟢 NIEDRIGE AUSWIRKUNG"]
                N1["Präsentations-Zeitverzug"]
            end
        end
        subgraph Wahrscheinlichkeit["📊 Wahrscheinlichkeit"]
            W1["Hoch: K8s-Komplexität, Zeitdruck"]
            W2["Mittel: Integration, Ressourcen"]
            W3["Niedrig: Präsentation"]
        end
    end
    classDef hoch fill:#d97968,stroke:#c06555,stroke-width:2px,color:#fff
    classDef mittel fill:#d4c171,stroke:#bfad60,stroke-width:2px,color:#2c3e50
    classDef niedrig fill:#9bc37d,stroke:#7aa65d,stroke-width:2px,color:#fff
    classDef info fill:#6366f1,stroke:#4f46e5,stroke-width:1px,color:#fff
    classDef transparent fill:none,stroke:none
    class H1,H2,H3,H4,H5 hoch
    class M1,M2,M3,M4,M5,M6,M7,M8,M9,M10 mittel
    class N1 niedrig
    class W1,W2,W3 info
    class Row1,Row2 transparent
```

## 1.4 Risiko-Matrix
Übersicht der Risiken nach Wahrscheinlichkeit und Auswirkung.
![alt text](image-1.png)


## 1.5 SWOT-Analyse 
Stärken, Schwächen, Chancen und Risiken des Projektes innerhalb der SWOT Analyse.

![alt text](image.png)

## 1.6 Sprint-Dokumentation
### 1.6.1 Sprint 1
#### **Zeitraum**

27.10.25 - 17.11.25

---

#### **Sprintziele**

	Repo Setup, Projektkonzipierung, Technisches Design

---


#### **User Stories mit Akzeptanzkriterien**
---

📍​**User Story 1:**


| Title:                   | Priority: | Estimate: |
| -------------------------- | ----------- | ----------- |
| Repo-Setup & Jira Setup | High      | 2h        |



Als Entwickler
Möchte ich **Meinen Text-Editor oder IDE zu meinem Github-Repo verknüpfen und meine Jira Seite für die User-Stories / Tasks vorbereiten**
damit ich **Ready bin, um das Projekt zu entwickeln und meinen Vortschritt festzuhalten**.

**Akzeptanzkriterien:**

- Ein verfügbares Repository für die Dokumentation der Semesterarbeit
- Präferierter IDE / Text-Editor welcher aufs Repo zugreifen kann und aktiv Änderungen vornimmt
- Meine User Stories im Jira festhalten

---

📍​**User Story 2:**


| Title:             | Priority: | Estimate: |
| -------------------- | ----------- | ----------- |
| Projektkonzipierung | High      | 1d        |



Als Projektleiterin
Möchte ich **Projektverlauf planen und die konzipierung verfassen**
damit ich **einen ersten Anhaltspunkt zum Architekturdesign habe, an welches sich das Projekt richten kann**.


**Akzeptanzkriterien:**

- Ein verfügbares KanBan Board mit den einzelnen Sprints und deren Ziele
- Die Funktionen Daten zu definieren und Cheklisten in den Zielen aufzubauen

---

📍​**User Story 3:**


| Title:              | Priority: | Estimate: |
| --------------------- | ----------- | ----------- |
| Technisches Design | Medium    | 1d        |

Als Architekt
Möchte ich **Einen ersten Entwurf meiner Grundarchitektur erstellen**
damit ich **meine Stakeholder den Fortschritt mitverfolgen können und ich Übersicht über die Aufgaben behalte**.
**Akzeptanzkriterien:**

- Ein Mermaid Diagramm mit der groben Vorstellung der Architektur
- Verständliche Beschriftung, Aufbau entsprechend der definierten Sachmittel

---

#### **Aufgabenübersicht Sprint 1**


| Aufgabe                  | Status              |
| -------------------------- | --------------------- |
| User Story 1 | Alternativ erledigt |
| User Story 2       | erledigt            |
| User Story 3    | erledigt            |

---

#### **Sprint Review**

⭐​​**Was wurde erreicht?**

- GitHub repo & Jira Setup erledigt
- Projektkonzipierung wurde erstellt
- Erster Entwurf für das Technische Design wurde erstellt

![alt text](image-2.png)
*_KanBan Angfangs Sprint_

![alt text](image-3.png)
*_KanBan Ende Sprint_

#### 🏔️​ **Herausforderungen**

- Jira Setup war sehr Mühsam. Mein Account war gesperrt und ich musste einen neuen Account sowie eine neue Site erstellen


#### 📚​ **Lessons Learned**

- Durch den Free-Tier von Jira ist man nur auf eine Domäne eingeschränkt
- Domänen und Sites sind zwei verschiedene Dinge
- Jira / Confluence Pages mit der Free-Tier werden nach ungefähr 6 Monaten gesperrt

---

#### **Retrospektive**


| **📈 More Of**                                                                                                                                                                                             | **📉 Less Of**                                                                                       | **✅ Keep Doing**                                                                                                                                                       | **🛑 Stop Doing**                                                                                                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Mehr Austausch mit Team-Kollegen und Collaboraters pflegen**<br>• Lösungen vergleichen und voneinander profitieren <br> | **Thema Microsoft Bookings**<br>• Via Bookings Termin früher Buchen. Slots sind schnell weg | **Offenheit für Tool-Empfehlungen** <br>• Visual Studio bietet wesentlich mehr Möglichkeiten als Obsidian <br><br>** Proaktive Lösungssuche bei Tool-Limitationen** | ***Kein Stop Doing Thema offen***<br>

#### **Ausblick auf Sprint 2**

- Wechsel / Migration des KanBan-Board - **Tool-Migration abschließen** - Vollständiger Wechsel zu Visual Studio
- Start Entwicklung der Grundarchitektur
- GUI Planung und erste Umsetzung
### 1.6.2 Sprint 2

#### **Zeitraum**

* Disclaimer: Anpassung der Technischen Lösung von DevOps Pipeline zu ArgoCD

17.11.25 - 15.12.25

---

#### **Sprintziele**

	Start Entwicklung Grundarchitektur; Verknüpfung aller Technischen Elemente sowie erste Testphase

---


#### **User Stories mit Akzeptanzkriterien**
---

📍​**User Story 4:**


| Title:                   | Priority: | Estimate: |
| -------------------------- | ----------- | ----------- |
| Entwicklung Grundarchitektur (AWS & Kubernetes) | High      | 2d        |



Als Entwickler
Möchte ich **Meine AWS EC2 Instanz aufsetzen sowie die Kubernetes Services für meine Microservices bereitstellen**
damit ich **Ready bin, um die Services zu Verknüpfen und ArgoCD zu initiieren**.

**Akzeptanzkriterien:**

- Eine verfügbare EC2 Instanz
- Installiertes Kubernetes auf der Instanz

---

📍​**User Story 5:**


| Title:             | Priority: | Estimate: |
| -------------------- | ----------- | ----------- |
| Verknüpfung der Technischen Elemente | High      | 2d        |



Als Entwickler
Möchte ich **Die Technischen Elemente (EC2, Kubernetes & ArgoCD, Deployment Manifests und deren Microservices)** bereitstellen
damit ich **auf neine erste funktionstüchtige ArgoCD Instanz zugreifen kann**.


**Akzeptanzkriterien:**

- Eine verfügbare ArgoCD GUI
- Ein gesundes cluster
- Erster Zugriff auf die Microservices

---
📍​**User Story 6:**


| Title:              | Priority: | Estimate: |
| --------------------- | ----------- | ----------- |
| ArgoCD Setup | Medium    | 1d        |

Als Entwickler
Möchte ich **Die Verfügbarkeit von ArgoCD gewährleisten**
damit ich **eine Übersicht auf meine aktiven Cluster sowie der Microservices erhalte**

**Akzeptanzkriterien:**

- WebGUI von Argo CD ersichtlich
---

#### **Aufgabenübersicht Sprint 2**


| Aufgabe                  | Status              |
| -------------------------- | --------------------- |
| User Story 1 | Alternativ erledigt |
| User Story 2       | In Progress         |
| User Story 3    | In Progress       |

---


📍​**User Story 7:**


| Title:              | Priority: | Estimate: |
| --------------------- | ----------- | ----------- |
| Testing | Medium    | 1d        |

Als Tester
Möchte ich **Die Verfügbarkeit und Funktionalitäten meiner Microservices testen**
damit ich **eine stabile Umgebung gewährleisten kann**

**Akzeptanzkriterien:**

- WebGUI von TrackMyGym ersichtlich
- Erstellung der Workout-Einträge möglich
- Wettervorhersagen entsprechend des Workouts verfügbar

---

#### **Aufgabenübersicht Sprint 2**


| Aufgabe                  | Status              |
| -------------------------- | --------------------- |
| User Story 4 | Erledigt |
| User Story 5       | In Progress         |
| User Story 6    | In Progress       |
| User Story 7    | In Progress       |

---

#### **Sprint Review**

⭐​​**Was wurde erreicht?**

- EC2 Instanz erstellt
- ...
- ...

![alt text](image-3.png)
*_KanBan Ende Sprint_

#### 🏔️​ **Herausforderungen**

- ...


#### 📚​ **Lessons Learned**

- ...

---

#### **Retrospektive**


| **📈 More Of**                                                                                                                                                                                             | **📉 Less Of**                                                                                       | **✅ Keep Doing**                                                                                                                                                       | **🛑 Stop Doing**                                                                                                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Mehr Austausch mit Team-Kollegen und Collaboraters pflegen**<br>• Lösungen vergleichen und voneinander profitieren <br> | **Thema Microsoft Bookings**<br>• Via Bookings Termin früher Buchen. Slots sind schnell weg | **Offenheit für Tool-Empfehlungen** <br>• Visual Studio bietet wesentlich mehr Möglichkeiten als Obsidian <br><br>** Proaktive Lösungssuche bei Tool-Limitationen** | ***Kein Stop Doing Thema offen***<br>

#### **Ausblick auf Sprint 3**

- ....
- ...
- ...
### 1.6.3 Sprint 3
#### **Zeitraum**

* Disclaimer: Anpassung der Technischen Lösung von DevOps Pipeline zu ArgoCD

15.12.25 - 28.01.25

---

#### **Sprintziele**

	Verbesserungen und Abschluss der Funktionalitäten, Vollendung der Dokumentation, Vorbereitung der Präsentation, Vollendung des Projekts & Abgabe

---


#### **User Stories mit Akzeptanzkriterien**
---

📍​**User Story 8:**


| Title:                   | Priority: | Estimate: |
| -------------------------- | ----------- | ----------- |
| Verbesserungen und Abschluss der Funktionalitäten | Medium      | 2d        |



Als Entwickler
Möchte ich **Allfällige Verbesserungen & Schönheitsmerkmale** umsetzen
damit ich **dem Projekt einen Feinschliff verleien kann (GUI, Zugriffe)**.

**Akzeptanzkriterien:**

- Eine GUI welches dem letzen Projekt gleich kommt
- Einfache Zugriffe auf die Instanz (Domänenname)
---

📍​**User Story 9:**


| Title:             | Priority: | Estimate: |
| -------------------- | ----------- | ----------- |
| Vollendung der Dokumentation | High      | 3d        |



Als Projektleiterin
Möchte ich **Meine Dokumentation auf dem Repo vollenden**
damit ich **Alle Themenbereiche des Projektes abgedeckt habe**.


**Akzeptanzkriterien:**

- Vollständige Dokumentation mit allen Überthemen auf dem aktuellen Repo

---
📍​**User Story 10:**


| Title:              | Priority: | Estimate: |
| --------------------- | ----------- | ----------- |
| Vorbereitung der Präsentation | Medium    | 1d        |

Als Sales Representative
Möchte ich **Eine Präsentation in Form eines Pitch** vorbereiten
damit ich **das Projekt den Stakeholdern vorstellen kann**

**Akzeptanzkriterien:**

- PowerPoint Präsentation mit live-Demo
---
📍​**User Story 10:**


| Title:              | Priority: | Estimate: |
| --------------------- | ----------- | ----------- |
| Vollendung des Projekts, Abgabe | Highest    | 1d        |

Als Projektleiter
Möchte ich **mein Projekt** abgeben
damit ich den Dozenten die Bewertung meines Projektes ermögliche.

**Akzeptanzkriterien:**

- Abgabe vollständiges Repo mit allen Dateien
- Abgabe PP Präsentation
- Abgabe allfällige Kommentare in Form eines Teams Posts
---

#### **Aufgabenübersicht Sprint 2**


| Aufgabe                  | Status              |
| -------------------------- | --------------------- |
| User Story 8 | offen |
| User Story 9       | In Progress         |
| User Story 10    | offen       |
| User Story 11    | offen       |



---

#### **Sprint Review**

⭐​​**Was wurde erreicht?**

- EC2 Instanz erstellt
- ...
- ...


*_KanBan Ende Sprint_

#### 🏔️​ **Herausforderungen**

- ...


#### 📚​ **Lessons Learned**

- ...

---

#### **Retrospektive**


| **📈 More Of**                                                                                                                                                                                             | **📉 Less Of**                                                                                       | **✅ Keep Doing**                                                                                                                                                       | **🛑 Stop Doing**                                                                                                                                                                                        |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Mehr Austausch mit Team-Kollegen und Collaboraters pflegen**<br>• Lösungen vergleichen und voneinander profitieren <br> | **Thema Microsoft Bookings**<br>• Via Bookings Termin früher Buchen. Slots sind schnell weg | **Offenheit für Tool-Empfehlungen** <br>• Visual Studio bietet wesentlich mehr Möglichkeiten als Obsidian <br><br>** Proaktive Lösungssuche bei Tool-Limitationen** | ***Kein Stop Doing Thema offen***<br>

#### **Ausblick auf Sprint 3**

- ....
- ...
- ...

# 2 Technische Dokumentation
## 2.1 Architektur Übersicht

Technische übersicht zur Migrierten Architektur:

```mermaid
graph TB
    %% External Users and Services
    User[👥 Benutzer<br/>HTTPS Zugriff]
    GitHub[🔄 GitHub Actions<br/>CI/CD Pipeline]
    WeatherAPI[☁️ OpenWeatherMap<br/>Weather API]
    
    %% AWS Cloud
    subgraph AWS["☁️ AWS Cloud (eu-central-1)"]
        subgraph EC2["🖥️ EC2 Instance (t3.medium)"]
            subgraph K8s["⎈ Kubernetes Cluster (k3s)"]
                
                %% Ingress
                Ingress[⚡ Nginx Ingress Controller<br/>Port 80/443]
                
                %% Kubernetes Services
                subgraph Namespace["📦 Namespace: trackmygym"]
                    Frontend[🎨 Frontend Pod<br/>React/Vue.js UI]
                    UserSvc[👤 User Service Pod<br/>Auth & Profile]
                    StatsSvc[📊 Stats Service Pod<br/>Analytics]
                    WorkoutSvc[💪 Workout Service Pod<br/>Training Plans]
                    WeatherSvc[🌤️ Weather Service Pod<br/>Weather Integration]
                    DB[(🗄️ PostgreSQL Pod<br/>users + workouts)]
                end
                
                %% Supporting Components
                HPA[📈 HPA<br/>Auto-Scaling]
            end
        end
    end
    
    %% Main User Flow
    User -->|HTTPS| Ingress
    Ingress -->|Routes| Frontend
    
    %% Frontend to Backend Services
    Frontend -->|API| UserSvc
    Frontend -->|API| StatsSvc
    Frontend -->|API| WorkoutSvc
    Frontend -->|API| WeatherSvc
    
    %% Services to Database
    UserSvc --> DB
    StatsSvc --> DB
    WorkoutSvc --> DB
    
    %% External API
    WeatherSvc -->|HTTP| WeatherAPI
    
    %% CI/CD Flow
    GitHub -->|Deploy| K8s
    
    %% Auto-Scaling
    HPA -.->|Scales| Namespace
    
    %% Styling
    classDef external fill:#e3f2fd,stroke:#1976d2,stroke-width:3px,color:#0d47a1
    classDef aws fill:#fff3e0,stroke:#f57c00,stroke-width:3px,color:#e65100
    classDef k8s fill:#e8f5e9,stroke:#43a047,stroke-width:3px,color:#2e7d32
    classDef service fill:#bbdefb,stroke:#1976d2,stroke-width:2px,color:#0d47a1
    classDef support fill:#fff9c4,stroke:#fbc02d,stroke-width:2px,color:#f57f17
    classDef db fill:#b3e5fc,stroke:#0288d1,stroke-width:3px,color:#01579b
    
    class User,GitHub,WeatherAPI external
    class AWS,EC2 aws
    class K8s,Namespace k8s
    class Frontend,UserSvc,StatsSvc,WorkoutSvc,WeatherSvc,Ingress service
    class HPA support
    class DB db
```

## 2.1 Architektur Übersicht - Angepasst

Nach Besprechnungen mit den Dozenten Philip Stark sowie Thanam Pangri bin ich auf die Idee einer Anpassung der Technischen Lösung gekommen.
Diese ist auf Positive Rückmeldung seitens der beiden Dozenten gestossen.

Anstatt der klassichen DevOps Pipelines via GitHub Actions, setze ich auf eine Umsetzung mit ArgoCD.

- Wieso ArgoCD?

ArgoCD bietet für den Zweck der Microservices eine deutlich übersichtliche Oberfläche für das Managen sowie des Überwachen der Cluster. Mittels der Self-Healing Funktionalitäten bieter ArgoCD somit eine stabile Lösung für den Gebrauch in einer Live-Umgebung.
ArgoCD gleicht sich ständig mit dem Repo ab als "Single Point of Truth". Alle commits sind nachvollziehbar.

ArgoCD bietet eine übersichtliche Web GUI, die den Zustand der Microservices, den Ressourcen und deren Beziehungen darstellt. So siehst man schnell, was deployed ist und wo es Probleme gibt.

Dies ist nach meiner Reflexion über meiner Technischen Planung eine passendere und nachhaltigere Lösung für meine Microservices.

Technische Übersicht zur ArgoCD Lösung:

```mermaid
graph TB
    %% External Users and Services
    User[👥 Benutzer<br/>HTTPS Zugriff]
    GitRepo[📁 Git Repository<br/>Manifests & Config]
    WeatherAPI[☁️ OpenWeatherMap<br/>Weather API]
    
    %% AWS Cloud
    subgraph AWS["☁️ AWS Cloud (eu-central-1)"]
        subgraph EC2["🖥️ EC2 Instance (t3.medium)"]
            subgraph K8s["⎈ Kubernetes Cluster (k3s)"]
                
                %% ArgoCD
                ArgoCD[🔄 ArgoCD<br/>GitOps Controller]
                
                %% Ingress
                Ingress[⚡ Nginx Ingress Controller<br/>Port 80/443]
                
                %% Kubernetes Services
                subgraph Namespace["📦 Namespace: trackmygym"]
                    Frontend[🎨 Frontend Pod<br/>React/Vue.js UI]
                    UserSvc[👤 User Service Pod<br/>Auth & Profile]
                    StatsSvc[📊 Stats Service Pod<br/>Analytics]
                    WorkoutSvc[💪 Workout Service Pod<br/>Training Plans]
                    WeatherSvc[🌤️ Weather Service Pod<br/>Weather Integration]
                    DB[(🗄️ PostgreSQL Pod<br/>users + workouts)]
                end
                
                %% Supporting Components
                HPA[📈 HPA<br/>Auto-Scaling]
            end
        end
    end
    
    %% Main User Flow
    User -->|HTTPS| Ingress
    Ingress -->|Routes| Frontend
    
    %% Frontend to Backend Services
    Frontend -->|API| UserSvc
    Frontend -->|API| StatsSvc
    Frontend -->|API| WorkoutSvc
    Frontend -->|API| WeatherSvc
    
    %% Services to Database
    UserSvc --> DB
    StatsSvc --> DB
    WorkoutSvc --> DB
    
    %% External API
    WeatherSvc -->|HTTP| WeatherAPI
    
    %% GitOps Flow
    GitRepo -->|Monitored by| ArgoCD
    ArgoCD -->|Sync & Deploy| Namespace
    ArgoCD -.->|Auto-Sync| Ingress
    
    %% Auto-Scaling
    HPA -.->|Scales| Namespace
    
    %% Styling
    classDef external fill:#e3f2fd,stroke:#1976d2,stroke-width:3px,color:#0d47a1
    classDef aws fill:#fff3e0,stroke:#f57c00,stroke-width:3px,color:#e65100
    classDef k8s fill:#e8f5e9,stroke:#43a047,stroke-width:3px,color:#2e7d32
    classDef service fill:#bbdefb,stroke:#1976d2,stroke-width:2px,color:#0d47a1
    classDef support fill:#fff9c4,stroke:#fbc02d,stroke-width:2px,color:#f57f17
    classDef db fill:#b3e5fc,stroke:#0288d1,stroke-width:3px,color:#01579b
    classDef argocd fill:#fce4ec,stroke:#c2185b,stroke-width:3px,color:#880e4f
    
    class User,WeatherAPI external
    class GitRepo argocd
    class AWS,EC2 aws
    class K8s,Namespace k8s
    class Frontend,UserSvc,StatsSvc,WorkoutSvc,WeatherSvc,Ingress service
    class HPA support
    class DB db
    class ArgoCD argocd
    
```

- Was sind die Hauptunterschiede?
- 1. DevOps Pipelines wurden in der Grafik entfernt
- 2. ArgoCD wurde in der Architekturübersicht hinzugefügt
- 3. ArgoCD wurde mit den Microservices verknüpft

  
 | Somit hat sich auch ein Element meiner Sprint Übersicht angepasst:

![alt text](image-3.png)


# 3. Deployment
## 3.1 AWS EC2 Setup

### Kostenmanagement
#### Billing-Alerts und threshholds für aktive Sessions
![alt text](image-5.png)


### EC2 Eigenschaften
#### Eigenschaften der Instanz

```
# - Instance Type: t3.medium oder größer (2 vCPU, 4 GB RAM minimum)
# - OS: Ubuntu 22.04 LTS
# - Storage: 30 GB SSD minimum
# - Security Group: Ports 22, 80, 443, 6443 (Kubernetes API)
```
![alt text](image-6.png)

#### Eigenschaften des Betriebssystem
![alt text](image-10.png)
#### User Data Eintrag
Damit das System auf dem neusten Stand bleibt
![alt text](image-8.png)


#### Eigenschaften der Security Group Regeln
```
Inbound Security Group Rules

SSH (bereits vorhanden)

Type: SSH
Port: 22
Source: My IP (oder 0.0.0.0/0)


HTTP

Type: HTTP
Port: 80
Source: Anywhere (0.0.0.0/0)


HTTPS

Type: HTTPS
Port: 443
Source: Anywhere (0.0.0.0/0)


Kubernetes

Type: Custom TCP
Port: 6443
Source: My IP (für kubectl Zugriff)
```
![alt text](image-9.png)

## 3.2 Kubernetes Setup
### K3S Installation
```
# Auf EC2 Instanz ausführen:
curl -sfL https://get.k3s.io | sh -

# kubectl konfigurieren
sudo cp /etc/rancher/k3s/k3s.yaml ~/.kube/config
sudo chown $USER ~/.kube/config

# Cluster Status prüfen
kubectl get nodes
```
![alt text](image-11.png)

### Bestehende Sudo Berechtigungen 

### Problem
Nach der k3s Installation konnte kubectl nicht ohne `sudo` verwendet werden, da die Standard-Konfigurationsdatei `/etc/rancher/k3s/k3s.yaml` nur für root lesbar ist.

### Lösung

#### Schritt 1: .kube Verzeichnis erstellen
```bash
mkdir -p ~/.kube
```

#### Schritt 2: k3s Konfiguration kopieren
```bash
sudo cp /etc/rancher/k3s/k3s.yaml ~/.kube/config
```

#### Schritt 3: Berechtigungen setzen
```bash
sudo chown ubuntu:ubuntu ~/.kube/config
chmod 600 ~/.kube/config
```

#### Schritt 4: KUBECONFIG Umgebungsvariable setzen
```bash
# Für die aktuelle Session
export KUBECONFIG=~/.kube/config

# Dauerhaft in .bashrc einfügen
echo 'export KUBECONFIG=~/.kube/config' >> ~/.bashrc

# .bashrc neu laden
source ~/.bashrc
```

#### Schritt 5: Funktionalität testen
```bash
kubectl get nodes
```

**Erwartete Ausgabe:**
```
NAME               STATUS   ROLES           AGE     VERSION
ip-172-31-27-185   Ready    control-plane   5d10h   v1.34.3+k3s1
```

#### Zusammenfassung

Nach diesen Schritten kann kubectl ohne `sudo` verwendet werden. Die KUBECONFIG Umgebungsvariable zeigt auf die Benutzerkopie der Konfiguration (`~/.kube/config`), die die korrekten Berechtigungen hat.

### Nützliche Befehle

```bash
# Cluster-Info anzeigen
kubectl cluster-info

# Alle Namespaces anzeigen
kubectl get namespaces

# Pods in einem Namespace anzeigen
kubectl get pods -n trackmygym

# Aktuelle Konfiguration anzeigen
kubectl config view
```


### Namespace erstellen

```bash
# TrackMyGym Namespace erstellen
kubectl create namespace trackmygym

# Überprüfen
kubectl get namespaces
```
![alt text](image-12.png)

### Repository Struktur
````
k8s/
├── apps/                           # Alle Microservices
│   ├── frontend/
│   │   ├── deployment.yaml         # Pod Definition + Container Image
│   │   ├── service.yaml            # Internes Networking
│   │   └── kustomization.yaml      # Optional: Config Management
│   ├── user-service/               # Gleiche Struktur für jeden Service
│   ├── workout-service/
│   ├── stats-service/
│   └── weather-service/
│
├── database/                       # PostgreSQL
│   ├── postgres-deployment.yaml    # Database Pod
│   ├── postgres-service.yaml       # Database Service
│   ├── postgres-pvc.yaml           # Persistent Storage
│   ├──postgres-configmap.yaml      # init.sql
|   └──postgres-secret.yaml         # DB Credentials
│
├── ingress/                        # Externes Routing
│   ├── ingress.yaml                # Traffic Regeln (welcher Host → welcher Service)
│   └── nginx-ingress-controller.yaml
│
├── argocd/                         # GitOps Konfiguration
│   ├── applications/               # ArgoCD Apps (eine pro Service)
│   │   ├── frontend-app.yaml
│   │   ├── user-service-app.yaml
│   │   └── ...
│   └── argocd-install.yaml
│
├── monitoring/                     # Auto-Scaling
│   └── hpa.yaml                    # Horizontal Pod Autoscaler Regeln
│
├── secrets/                        # Sensitive Daten (NICHT in Git!)
│   └── README.md
│
├── .gitignore                      # Verhindert Secrets-Commit
└── README.md                       # Projektdokumentation
````


| Datei | Zweck |
|-------|-------|
|` deployment.yaml` | Definiert WAS läuft (Image, Replicas, Resources) |
|`service.yaml` | Macht Pods intern erreichbar (Networking) |
|`ingress.yaml` | Macht Services von außen erreichbar (HTTP Routing) |
|`argocd/*-app.yaml` | Sagt ArgoCD: "Deploy diesen Ordner automatisch" |
|`hpa.yaml` | Auto-Scaling bei Last |

### Docker Registry

- Registry-Anbieter: `hub.docker.com`
- Username: `gitlilia`

### Docker-Build Befehle
````
# Alle Images bauen
cd ICTNE24_Semesterarbeit3_L.M # Aus dem letzten Repo

docker build -t gitlilia/trackmygym-frontend:v1.0.0 ./frontend
docker build -t gitlilia/trackmygym-user-service:v1.0.0 ./user-service
docker build -t gitlilia/trackmygym-workout-service:v1.0.0 ./workout-service
docker build -t gitlilia/trackmygym-stats-service:v1.0.0 ./stats-service
docker build -t gitlilia/trackmygym-weather-service:v1.0.0 ./weather-service
docker build -t gitlilia/trackmygym-nginx:v1.0.0 ./nginx
````
#### Nachweis Build-Prozess
![alt text](image-13.png)
#### Nachweis Build-Prozess Erfolgreich
![alt text](image-14.png)

````
# Alle Images pushen
docker push gitlilia/trackmygym-frontend:v1.0.0
docker push gitlilia/trackmygym-user-service:v1.0.0
docker push gitlilia/trackmygym-workout-service:v1.0.0
docker push gitlilia/trackmygym-stats-service:v1.0.0
docker push gitlilia/trackmygym-weather-service:v1.0.0
docker push gitlilia/trackmygym-nginx:v1.0.0
````

#### Nachweis Push-Prozess
![alt text](image-15.png)
#### Nachweis Push-Prozess Erfolgreich
![alt text](image-16.png)
#### Docker-Hub Übersicht
- ✅ trackmygym-frontend
- ✅ trackmygym-user-service
- ✅ trackmygym-workout-service
- ✅ trackmygym-stats-service
- ✅ trackmygym-weather-service
- ✅ trackmygym-nginx
  
![alt text](image-17.png)


### Kubernetes Manifests
# Kubernetes Manifests Übersicht

| Kategorie | Komponente | Dateien |
|-----------|------------|---------|
| **1. PostgreSQL (Database)** | Database | • Deployment / StatefulSet<br>• Service<br>• PersistentVolumeClaim (Speicher)<br>• ConfigMap (init.sql)<br>• Secret (DB Passwort) |
| **2. Microservices** | Frontend<br>User Service<br>Workout Service<br>Stats Service<br>Weather Service | • deployment.yaml<br>• service.yaml<br><br>*(pro Service)* |
| **3. Nginx Ingress** | Ingress Controller | • ingress.yaml (mit sslip.io)<br>• nginx-ingress-controller.yaml |
| **4. ArgoCD Applications** | GitOps | • frontend-app.yaml<br>• user-service-app.yaml<br>• workout-service-app.yaml<br>• stats-service-app.yaml<br>• weather-service-app.yaml<br>• database-app.yaml |
| **5. Monitoring** | Auto-Scaling | • HPA (Horizontal Pod Autoscaler) |