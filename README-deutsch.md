# UBlock-Origin Erlaubt-Liste
UBlock-Origin Javascript Filterliste, um den Wechsel für alle zu erleichtern

[english text](https://github.com/boredsquirrel/ublock-allowlist/blob/main/README.md)

Dieses Repo enthält "UBlock Origin dynamische Filterregeln". Kurzgesagt, ist es ein besserer Ersatz für [NoScript](https://noscript.net)

## Ziel
UBlock-Origin funktioniert okay als Werbeblocker, wobei es "badness enumeration" verwendet, mit riesigen Listen an Domains. Aber dieses Konzept ist zum Scheitern verurteilt, also müssen wir

1. Jede Art von ausführbarem Code anfangs blockieren
2. Manuell Code von vertrauten Ursprüngen freigeben

Dieses Projekt soll bei diesem mühsamen Prozess helfen, indem es einen großen Vorspung gibt, ein "kleines Internet" sozusagen.

## Einfärbung dieser Liste
Ich bin ein deutscher Typ, interessiere mich für Technik und Naturwissenschaften. Das wird durch die Filterliste recht klar, weil sie ja quasi meine Browser-Historie ist (*Ich hoffe ihr wertschätzt das*).

Du kannst gerne beliebige Seiten ergänzen, um diesen Fokus aufzuweichen, aber bitte folge diesen Regeln:

## Regeln

### 1. Bilder sind erlaubt

### 2. Alles Javascript ist standardmäßig blockiert
Das beinhält 1st und 3rd party Javascript

### 3. Keine Quellen werden blockiert
URLs werden nur erlaubt wenn du ihnen vertraust. Doppelt blockieren bringt keinen Vorteil.

### 4. Wie man erlaubt
UBlock Origin zeigt 2 Spalten an:

![screenshot](https://github.com/boredsquirrel/ublock-allowlist/blob/main/images/ubo-popups.jpg?raw=true)

Die linke Spalte gilt für jede beliebige Website, z. B. „lade `google.com` Javascript auf jeder Website“. Die rechte Spalte bezieht sich auf die aktuell geöffnete Website, z. B. „Lade `google.com` Javascript nur auf `youtube.com`.

Beim Erlauben, beschränk bekannte Überwachungsquellen (wie Google, Facebook, Amazon usw.) auf ihre eigenen Homepages.

Um die Liste kürzer zu machen, kannst du das Javascript beliebiger Websites in der linken Spalte freischalten, da es „vertrauenswürdig“ ist und nicht auf anderen Websites geladen wird.

### 5. Was soll freigeschaltet werden?
Sicherheit ist ein Gleichgewicht zwischen „alles lädt, was es will“ und „ich sehe eine leere Seite“.

Das bedeutet, dass viele CDNs und andere zentralisierte Akteure im Web freigeschaltet werden müssen, da eine Vielzahl von Websites auf sie angewiesen ist.

Aber experimentiere gerne, gebe nicht einfach alles frei. Ein paar fehlende Bilder können in Ordnung sein, und einige laden vielleicht nicht einmal etwas Nützliches, sondern nur Analytics usw.

## Einrichten
1. Installiere UBlock Origin, d.h. du brauchst Firefox oder einen Firefox-basierten Browser (Mull, Torbrowser, MullvadBrowser, Midori, Floorp, Zen...)
2. Aktivier in den UBO-Einstellungen den „erweiterten Modus“.

![Bildschirmfoto](https://github.com/boredsquirrel/ublock-allowlist/blob/main/images/ubo-advanced-enable.jpg?raw=true)

3. Nun kannst du diese Liste unter „Meine Regeln“ importieren
4. Öffne einige Websites, mit dem Addon-Popup (siehe erster Screenshot) kannst du Javascript freischalten
5. Diese Freischaltungen sind temporär !!! (Aus welchem Grund auch immer). Gehe auf die UBO-Einstellungsseite, „Meine Regeln“ und „Commite“ deine Änderungen in die Liste

![screenshot](https://github.com/boredsquirrel/ublock-allowlist/blob/main/images/ubo-settings.jpg?raw=true)

## Wie man mithilft
Sobald du alles eingerichtet hast, kannst dz weitere vertrauenswürdige Javascript-Quellen freischalten und die Änderungen committen.

UBO wird eine ordentliche Liste daraus machen.

1. Forke dieses Repo
2. Stelle sicher, dass du die aktuelle Liste als Basis verwendest, sonst können Änderungen verloren gehen
3. Verwende in deinem Fork einfach den Github Web Editor und bearbeite die Blockliste
4. Ersetze den gesamten Inhalt durch deine neue Liste
5. Committe und erstelle einen neuen Branch. Verwende irgendeinen Namen für diesen Zweig
6. Gehe zurück zu diesem Repository, nicht zu deinem Fork
7. Benutze das Popup in Github, um einen PR zu erstellen, von deinem Fork und Branch, zu diesem Repo und dem `main` Branch
8. Schreibe ein paar Worte, und wir können es schnell zusammenführen!
