# GitBook-HTMLCSS

| **Autoren**                      | Kiara Baldo, Flurin Kläy, Mikolaj Spychala, Simon Kaiser |
|----------------------------------|-----------------------------------------------------------|
| **Klasse**                       | 5ia24c                                                    |
| **Lehrperson**                   | Selina Gahlinger                                          |
| **Abgabetermine**                | 01.07.2025                                                |

## 📖 Inhaltsverzeichnis

1. [Einführung in HTML & CSS](#einführung-in-html--css)  
2. [HTML-Grundlagen](#html-grundlagen)  
3. [CSS-Grundlagen](#css-grundlagen)  
4. [Layout & Positionierung](#layout--positionierung)  
5. [Responsive Design](#responsive-design)  
6. [Übungen](#übungen)  
7. [Glossar](#glossar)  
8. [Ressourcen & Links](#ressourcen--links)

---

## Einführung in HTML & CSS

HTML und CSS bilden das Grundgerüst jeder modernen Webseite.  
- **HTML (HyperText Markup Language)** strukturiert den Inhalt.
- **CSS (Cascading Style Sheets)** gestaltet das Aussehen.

👉 **Beispiel:**  
```html
<!DOCTYPE html>
<html>
<head>
  <title>Meine erste Seite</title>
  <style>
    body { background-color: lightblue; }
  </style>
</head>
<body>
  <h1>Hallo Welt!</h1>
  <p>Willkommen auf meiner Webseite.</p>
</body>
</html>

## 📄 HTML-Grundlagen

### 🔹 Aufbau eines HTML-Dokuments

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Titel der Seite</title>
  </head>
  <body>
    <!-- Inhalt kommt hier hin -->
  </body>
</html>
🔹 Wichtige Tags
Tag	Bedeutung
<h1>	Überschrift
<p>	Absatz
<a>	Link
<img>	Bild
<ul>	Ungeordnete Liste
<ol>	Geordnete Liste
<li>	Listenelement
<table>	Tabelle
🎨 CSS-Grundlagen
🔹 Einbindung von CSS
Im HTML direkt:

html
Kopieren
Bearbeiten
<style>
  p { color: red; }
</style>
Extern per Datei:

html
Kopieren
Bearbeiten
<link rel="stylesheet" href="style.css">
🔹 Selektoren und Eigenschaften
css
Kopieren
Bearbeiten
/* Selektoren */
h1 {
  color: blue;
  font-size: 32px;
}

.container {
  background-color: #eee;
}

#hauptbereich {
  padding: 20px;
}
🧱 Layout & Positionierung
🔹 Box-Modell
Jedes HTML-Element ist eine Box:

csharp
Kopieren
Bearbeiten
[Margin]
  [Border]
    [Padding]
      [Content]
🔹 Flexbox Beispiel
CSS:

css
Kopieren
Bearbeiten
.container {
  display: flex;
  justify-content: space-between;
}
HTML:

html
Kopieren
Bearbeiten
<div class="container">
  <div>Box 1</div>
  <div>Box 2</div>
</div>
🔹 Grid Beispiel
css
Kopieren
Bearbeiten
.grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
}
📱 Responsive Design
🔹 Media Queries
css
Kopieren
Bearbeiten
@media (max-width: 600px) {
  body {
    background-color: yellow;
  }
}
Webseiten sollen auf allen Geräten gut aussehen.

Verwende relative Einheiten wie %, em, vh, vw anstelle fester Pixel (px).

🧪 Übungen
HTML-Grundstruktur schreiben

Ein Bild und Link einbauen

Liste mit 3 Punkten

Eigene CSS-Datei erstellen

Flexbox Layout mit 2 Spalten

Navigation mit Hover-Effekt

Formular mit Eingabefeldern

Grid-Galerie

Tabelle gestalten

Seite responsive machen


