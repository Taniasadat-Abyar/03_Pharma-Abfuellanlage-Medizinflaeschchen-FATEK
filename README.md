# Pharmazeutischer Reinraum-Isolator (lokal konstruiert, Iran-Erstentwicklung)
**Auftraggeber:** Kianmehr Pharma / Universität Teheran (Rang 1 in Iran)  
**Durchgeführt über:** Koosha Sanat Farmad, Teheran  
**Zeitraum:** 2014 – 2020 (Projektbasis)  
**Rolle:** SPS-Programmiererin, HMI-Entwicklerin, Inbetriebnahme-Ingenieurin

---

## 📌 Projektübersicht

Inbetriebnahme, Entwicklung, Programmierung und Visualisierung des **ersten lokal konstruierten pharmazeutischen Isolators in Iran** – unabhängig von Importprodukten. Das System dient der **Krebszellforschung** an der Universität Teheran unter strengen GMP-Anforderungen (Good Manufacturing Practice).

Der Isolator ist ein **zweiteiliges System**:
- **Passkasten** (Schleuse für Materialeinschleusung)
- **Hauptkasten** (sterile Arbeitsumgebung für pharmazeutische Reinraumanwendungen)

---

## 🛠️ Eingesetzte Technologien & Werkzeuge

| Bereich | Technologie |
|---|---|
| SPS | Siemens S7-200 |
| HMI / Visualisierung | Easy View HMI |
| Regelung | PID-Regelkreise |
| Norm | GMP (Good Manufacturing Practice) |
| Branche | Pharmaindustrie / Medizinische Forschung |

---

## 💡 Konzepte & Aufgabenbereiche

### 1. Systemkonzept – Zweiteiliger Isolator

#### Passkasten (Schleuse)
- Druckgeregelte Schleusenkammer zur Materialeinschleusung
- Desinfektion und Druckausgleich vor Öffnung zur Hauptkammer
- Verriegelungslogik: Sicherstellung, dass nie beide Türen gleichzeitig offen sind

#### Hauptkasten (Sterile Arbeitskammer)
- Sterile, überwachte Umgebung für pharmazeutische Forschungsarbeiten (Krebszellen)
- Kontinuierliche Überwachung und Regelung von Druck, Temperatur und relativer Luftfeuchtigkeit
- HEPA-Filtration und Luftstromüberwachung

### 2. SPS-Programmierung (Siemens S7-200)
- Gesamtsteuerung des Isolators mit **Siemens S7-200**
- Ablaufsteuerung für Einschleusungsprozess (Passkasten)
- Überwachungslogik für kritische Prozessparameter
- Alarmmanagement bei Über- / Unterschreitung von Grenzwerten
- Verriegelungslogiken für Sicherheit des Reinraums

### 3. PID-Regelkreise (Prozessregelung)
Drei unabhängige **PID-Regelkreise** gemäß GMP-Anforderungen:

| Regelgröße | Stellgröße | Anforderung |
|---|---|---|
| Druck | Ventil / Gebläse | Überdruck gegenüber Umgebung (Schutz vor Kontamination) |
| Temperatur | Heizung / Kühlung | Konstante Arbeitstemperatur |
| Relative Luftfeuchtigkeit | Befeuchter / Entfeuchter | Definierter RH-Bereich |

- Parameterierung (P, I, D-Anteile) und Inbetriebnahme der Regelkreise
- Stabilitätsoptimierung für präzise und schwingungsfreie Regelung

### 4. HMI-Visualisierung (Easy View)
- Prozessvisualisierung beider Kammern (Passkasten + Hauptkasten)
- Echtzeit-Anzeige aller Regelgrößen (Druck, Temperatur, Luftfeuchtigkeit)
- Trendanzeige für Langzeitüberwachung
- Alarmübersicht mit Quittierung
- Protokollierung der Messwerte (GMP-Dokumentationsanforderung)

---

## 🔄 Prozessablauf Einschleusung

```
Material bereitstellen (außen)
        ↓
Passkasten öffnen (Außentür)
        ↓
Material einlegen → Außentür schließen
        ↓
Desinfektion & Druckangleich im Passkasten
        ↓
Verriegelung prüfen (Sicherheitslogik)
        ↓
Innentür öffnen → Material in Hauptkasten
        ↓
Innentür schließen
        ↓
Kontinuierliche PID-Regelung (Druck / Temp / RH)
```

---

## 📈 Besondere Bedeutung & Ergebnisse

- **Erster lokal konstruierter Isolator in Iran** – importunabhängig und damit strategisch bedeutsam
- Einsatz an der **Universität Teheran (Rang 1 in Iran)** für Krebszellforschung
- GMP-konforme Prozessführung und Dokumentation
- Stabiler Dauerbetrieb unter strengsten Reinraumbedingungen
- Nachweis, dass lokale Entwicklung internationalen Pharmastandards entsprechen kann
