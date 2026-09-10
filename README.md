# Web Application Security Dashboard

> **Work in Progress**  
> Dieses Projekt befindet sich aktuell in aktiver Entwicklung. Die bestehende Funktionalität wird kontinuierlich erweitert.

## Dashboard Demo

**[Dashboard Demo](https://marco-devspace.github.io/dashboard-demo/)**

Die Dashboard Demo zeigt einen Ausschnitt des vollständigen **Web Application Security Dashboards** und verwendet statische Beispieldaten zur Veranschaulichung der Benutzeroberfläche und Funktionen. <br>
Der vollständige Funktionsumfang befindet sich aktuell in aktiver Entwicklung.

---

## Über das Projekt

Das **Web Application Security Dashboard** dient zur zentralen Darstellung und Auswertung von Security-Scans für mehrere Webseiten.

Ein separater **Web Application Security Scanner** untersucht Webseiten auf potenzielle Sicherheitsrisiken, klassifiziert die gefundenen Schwachstellen und erstellt daraus einen PDF-Report.

Die Scan-Ergebnisse werden in einer **MySQL-Datenbank** gespeichert und anschließend über das Web Application Security Dashboard ausgewertet.

Zu den wichtigsten Funktionen gehören der **Security Score**, die Entwicklung des Scores über die Zeit, eine Scan-Historie, eine Übersicht der gefundenen Schwachstellen, ein Change Log sowie die Verwaltung mehrerer Webseiten.

---

## Features

### Bereits umgesetzt

- [x] Web Application Security Scanner für öffentlich erreichbare Webseiten
- [x] Speicherung der Scan-Ergebnisse in MySQL
- [x] Security Score auf Basis der gefundenen Schwachstellen
- [x] Score-Entwicklung als Graph
- [x] Verwaltung mehrerer Webseiten
- [x] Übersicht der letzten Scans
- [x] Change Log für neue und behobene Schwachstellen
- [x] Generierung von PDF-Security-Reports
- [x] Verlinkung des letzten PDF-Reports im Web Application Security Dashboard
- [x] Docker-Unterstützung für Frontend, Backend und Datenbank

### Noch geplant

- [ ] Authentifizierung mit Auth0
- [ ] Admin-Bereich mit Benutzer- und Websiteverwaltung
- [ ] Automatisierte wöchentliche Security-Scans
- [ ] E-Mail-Benachrichtigungen bei neuen Scanergebnissen

---

## Technologie-Stack

- **Frontend:** Angular, TypeScript, SCSS
- **Backend:** Python, FastAPI, SQLAlchemy
- **Datenbank:** MySQL
- **Web Application Security Scanner:** Python
- **Infrastruktur:** Docker
- **Deployment:** GitHub Pages (Demoversion)

---

## Ziel

Das langfristige Ziel ist eine Plattform zur **kontinuierlichen Überwachung potenzieller Sicherheitsprobleme mehrerer Webseiten**.

Der aktuelle manuelle Ablauf soll schrittweise zu einem automatisierten Prozess erweitert werden:

```text
Wöchentlicher Scan
       ↓
Web Application Security Scanner
       ↓
Scan-Ergebnisse + PDF Report
       ↓
MySQL / FastAPI
       ↓
Web Application Security Dashboard
       ↓
Score & Change Log
       ↓
E-Mail-Benachrichtigung
```
