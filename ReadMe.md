# 🕒 AzubiTracker – Zeiterfassung für Auszubildende

**AzubiTracker** ist eine moderne, einfache Anwendung zur **Zeiterfassung in der Ausbildung**.  
Mit einer intuitiven Benutzeroberfläche und einer zuverlässigen lokalen Datenbank ermöglicht sie Auszubildenden, ihre täglichen Tätigkeiten, Arbeitszeiten und Ausbildungsorte effizient zu dokumentieren – z. B. für das IHK-Berichtsheft oder persönliche Nachweise.

---

## 🚀 Features

- 📅 **Tägliche Zeiterfassung** (Start-/Endzeit, Aufgabe, Ort)
- 📋 **Eintragsliste mit Wochen-/Monatsübersicht**
- ✍️ **Bearbeiten & Löschen von Einträgen**
- 📤 **Export-Funktion (CSV, optional PDF)**
- 📊 **Auswertung nach Zeitraum (optional)**
- 🌐 **React + TypeScript Frontend**
- 🐍 **Flask API + SQLite Backend**
- 🔐 Lokale Speicherung – keine Cloud notwendig

---

## 🛠 Tech-Stack

| Bereich   | Technologie              |
|-----------|---------------------------|
| Frontend  | React, TypeScript, Axios  |
| Backend   | Flask, SQLite, flask-cors |
| Datenbank | SQLite (lokal, portabel)  |
| API       | REST (JSON-basiert)       |

---

## 📁 Projektstruktur

azubitracker/
├── backend/ # Flask + SQLite
│ ├── app.py
│ └── entries.db
└── frontend/ # React + TypeScript
├── src/
├── public/
└── package.json

yaml
Kopieren
Bearbeiten

---

## 🧪 Beispiel-Eintrag

```json
{
  "date": "2025-07-25",
  "start_time": "08:00",
  "end_time": "16:30",
  "task": "Fehlersuche im Backend",
  "location": "Betrieb"
}
```

## ▶️ Lokales Setup
📦 Backend starten (Flask)

```bash
cd backend
pip install flask flask-cors
python app.py
```
## 🌐 Frontend starten (React)
```bash
cd frontend
npm install
npm run dev  # oder: npm start
```
Standard-API: http://localhost:5000
Frontend: http://localhost:5173 (Vite) oder 3000 (Create React App)

## 📤 Geplante Erweiterungen
- 🧾 PDF-Export fürs Berichtsheft (IHK-konform)
- 🔐 Login & Passwortschutz
- 🔁 Aufgaben-Vorlagen & automatische Wochenberichte
- 📱 Mobile-Ansicht / PWA-Unterstützung