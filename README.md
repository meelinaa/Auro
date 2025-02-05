# Auro: Virtueller Aktien-Broker 📈
<img src="/README-images/banner.png" alt="Beschreibung" style="width: 100%; display: block;">

Auro ist eine interaktive Webanwendung, mit der Benutzer Aktien suchen, deren Live-Daten und weitere Informationen einsehen sowie diese kaufen und verkaufen können. Benutzer haben Zugriff auf ein persönliches Konto mit einem bestimmten Guthaben, um Transaktionen durchzuführen. Die Anwendung umfasst sowohl ein modernes Frontend als auch ein leistungsstarkes Backend.

## Features

- **Aktieninformationen:** Durchsuchen Sie eine große Auswahl an Aktien und erhalten Sie Live-Daten und Details.
- **Portfolio-Management:** Kaufen und verkaufen Sie Aktien und verwalten Sie Ihr persönliches Portfolio.
- **Benutzerkonto:** Verfolgen Sie Ihr Guthaben und Ihre Transaktionen.
- **Reaktionsschnelles Frontend:** Entwickelt mit React, HTML und CSS für eine intuitive Benutzeroberfläche.
- **Backend-Integration:** RESTful APIs für die Kommunikation zwischen Frontend und Backend.
- **Datenbank:** Speicherung und Verwaltung der Daten mit PostgreSQL, bereitgestellt via Docker.
- **Business-Logik:** Verwaltung von Transaktionen, Portfolio-Berechnungen und Validierungen im Backend.
- **Testing:** Unit-Tests wurden bereits hinzugefügt, Integrationstests folgen in einer späteren Iteration.
- **Echte Business-Anwendung:** Das Projekt simuliert reale Szenarien aus der Finanzwelt und bietet praxisnahe Funktionen für ein Portfolio-Management-System.
- **Web Scraping:** Integration von JSoup, um zusätzliche Finanzdaten von Webseiten zu extrahieren und im System verfügbar zu machen.
- **Skalierbarkeit:** Die Architektur des Projekts wurde so entworfen, dass zukünftige Erweiterungen und neue Funktionen problemlos integriert werden können.


## Projektstruktur

Da Frontend und Backend in separaten Repositories gepflegt werden, finden Sie die aktuellen Inhalte hier:
- [Frontend Repository](https://github.com/meelinaa/ProjektAuroFrontend)  
- [Backend Repository](https://github.com/meelinaa/ProjektAuro)


## Technologien

- ⚛️ **Frontend:** React (JavaScript ES6+, HTML, CSS)  
  Entwickelt für eine dynamische und reaktionsschnelle Benutzeroberfläche.
- ☕ **Backend:** Java mit Spring Boot, Spring Data JPA, Lombok  
  Enthält die gesamte Business-Logik sowie Datenbank-Integrationen. Sicherheitsfunktionen wie Authentifizierung und Autorisierung sind derzeit nicht implementiert, können jedoch in zukünftigen Iterationen hinzugefügt werden.
- 🔗 **API:** RESTful Services  
  Schnittstelle zur Kommunikation zwischen Frontend und Backend.
- 🗄️ **Datenbank:** PostgreSQL (via Docker)  
  Speicherung und effiziente Verwaltung aller Daten.
- 🐳 **Containerisierung:** Docker  
  Für eine portable und einfache Bereitstellung der Anwendung.
- ✅ **Testing:**  
  Unit-Tests wurden hinzugefügt, Integrationstests folgen in einer späteren Phase.


## Software-Entwicklung und Planung

Dieses Projekt wurde vollständig von Grund auf selbst geplant und entwickelt. Dazu gehören:

- **Planung und Architektur:** Erstellung der gesamten Software-Architektur, einschließlich der Backend- und Frontend-Struktur.
- **Coding-Praktiken:** Verwendung von Clean Code-Prinzipien und bewährten Design Patterns, um wartbaren und skalierbaren Code sicherzustellen.
- **Iterative Entwicklung:** Features werden schrittweise hinzugefügt und verbessert, basierend auf einem agilen Entwicklungsansatz.
- **Lernfokus:** Dieses Projekt wurde entwickelt, um meine Fähigkeiten in der Softwareentwicklung zu vertiefen, einschließlich Frontend- und Backend-Integration, API-Entwicklung, Datenbankmanagement und mehr.


## Screenshots

1. **Startseite / Portfolio:** Übersicht des Portfolios und weiteren empfolenen Aktien.
<img src="/README-images/portfolio.png" alt="Beschreibung" style="width: 100%; display: block;">
2. **Aktieninformationen:** Details und Grafiken zu einer ausgewählten Aktie.
<img src="/README-images/aktie.png" alt="Beschreibung" style="width: 100%; display: block;">
3. **Kauf-/Verkauf-Ansicht:** Eingabemaske für den Handel von Aktien.
<img src="/README-images/kaufen.png" alt="Beschreibung" style="width: 40%; display: flex;">
<img src="/README-images/bestätigen.png" alt="Beschreibung" style="width: 40%; display: flex;">
4. **Transaktionshistorie:** Übersicht über durchgeführte Käufe und Verkäufe.
<img src="/README-images/konto.png" alt="Beschreibung" style="width: 100%; display: block;">


## Voraussetzungen

Um dieses Projekt lokal auszuführen, benötigen Sie folgende Tools:

1. [Node.js](https://nodejs.org/) (LTS-Version empfohlen)
2. [Docker](https://www.docker.com/)
3. Java 17 oder höher
4. Maven (für Backend-Builds)
5. Git (zum Klonen des Repositories)


## Lokale Installation und Ausführung

### 1. Projekt klonen
```bash
 git clone https://github.com/dein-benutzername/auro.git
 cd auro
```

### 2. Backend starten

1. **Docker Compose ausführen:**

   Navigieren Sie in das Backend-Verzeichnis und starten Sie die Datenbank::
   ```bash
   docker-compose up -d
   docker run --name auro_postgres -e POSTGRES_USER=Auro1234 -e POSTGRES_PASSWORD=passwordAuro -e POSTGRES_DB=databaseAuro -p 5432:5432 -d postgres
   ```

2. **Backend mit Maven starten:**

   Öffnen Sie ein neues Terminal im Backend-Verzeichnis und führen Sie folgendes aus:
   ```bash
   mvn spring-boot:run
   ```

   Das Backend wird standardmäßig unter `http://localhost:8080` ausgeführt.

### 3. Frontend starten

1. **Abhängigkeiten installieren:**

   Wechseln Sie ins Frontend-Verzeichnis:
   ```bash
   cd frontend
   npm install
   ```

2. **Frontend starten:**

   ```bash
   npm start
   ```

   Das Frontend wird standardmäßig unter `http://localhost:3000` ausgeführt.

---

## Nutzung

1. Besuchen Sie die URL `http://localhost:3000` in Ihrem Browser.
2. (geplant) Registrieren oder melden Sie sich an, um auf die Funktionen zuzugreifen.
3. Suchen Sie nach Aktien, fügen Sie diese Ihrem Portfolio hinzu und verfolgen Sie Ihre Transaktionen.


## Lizenz
Dieses Projekt steht unter der [MIT-Lizenz](LICENSE).

---

## Kontakt
Für Fragen oder Feedback kontaktieren Sie mich über [E-Mail](mailto:melinakiefer@hotmail.de) oder GitHub.
