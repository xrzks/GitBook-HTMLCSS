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
6. [Übungen](#Übungen)  
7. [Glossar](#glossar)  
8. [Ressourcen & Links](#ressourcen--links)

---

## Einführung in HTML & CSS

HTML und CSS bilden das Grundgerüst jeder modernen Webseite.  
- **HTML (HyperText Markup Language)** strukturiert den Inhalt.  
- **CSS (Cascading Style Sheets)** gestaltet das Aussehen.

🔎 **Beispiel:**  
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
```

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
```

### 🔹 Wichtige Tags

| Tag       | Bedeutung            |
|-----------|----------------------|
| `<h1>`    | Überschrift          |
| `<p>`     | Absatz               |
| `<a>`     | Link                 |
| `<img>`   | Bild                 |
| `<ul>`    | Ungeordnete Liste    |
| `<ol>`    | Geordnete Liste      |
| `<li>`    | Listenelement        |
| `<table>` | Tabelle              |

## 🎨 CSS-Grundlagen

### 🔹 Einbindung von CSS

**Im HTML direkt:**
```html
<style>
  p { color: red; }
</style>
```

**Extern per Datei:**
```html
<link rel="stylesheet" href="style.css">
```

### 🔹 Selektoren und Eigenschaften

```css
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
```

## 🧱 Layout & Positionierung

### 🔹 Box-Modell

Jedes HTML-Element ist eine Box:
```
[Margin]
  [Border]
    [Padding]
      [Content]
```

### 🔹 Flexbox Beispiel

**CSS:**
```css
.container {
  display: flex;
  justify-content: space-between;
}
```

**HTML:**
```html
<div class="container">
  <div>Box 1</div>
  <div>Box 2</div>
</div>
```

### 🔹 Grid Beispiel
```css
.grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
}
```

## 📱 Responsive Design

### 🔹 Media Queries
```css
@media (max-width: 600px) {
  body {
    background-color: yellow;
  }
}
```

Webseiten sollen auf allen Geräten gut aussehen.  
Verwende relative Einheiten wie %, em, vh, vw anstelle fester Pixel (px).

## 🧪 Übungen

(Die Lösungen sind im nächsten Kapitel zu finden.)

1. HTML-Grundstruktur schreiben  
2. Ein Bild und Link einbauen  
3. Liste mit 3 Punkten  
4. Eigene CSS-Datei erstellen  
5. Flexbox Layout mit 2 Spalten  
6. Navigation mit Hover-Effekt  
7. Formular mit Eingabefeldern  
8. Grid-Galerie  
9. Tabelle gestalten  
10. Seite responsive machen

## 🧪 Übungen mit Lösungen & Erklärungen

(Einzelne Aufgaben siehe vorherige Nachricht – Inhalt zu lang für diese Antwort)
```

}

