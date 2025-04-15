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

# 🧪 Übungen mit Lösungen & Erklärungen

---

## ✅ Übung 1: HTML-Grundstruktur schreiben

**Aufgabe:** Erstelle ein HTML-Dokument mit Grundstruktur, Überschrift und Absatz.

### 💡 Lösung:
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Meine erste Seite</title>
  </head>
  <body>
    <h1>Hallo Welt!</h1>
    <p>Das ist mein erster Absatz in HTML.</p>
  </body>
</html>
```

🧠 **Erklärung:**
- `<!DOCTYPE html>`: Gibt an, dass es sich um HTML5 handelt.
- `<html>` umschließt die gesamte Seite.
- `<head>` enthält Metadaten wie den Seitentitel.
- `<body>` enthält den sichtbaren Inhalt.

---

## ✅ Übung 2: Ein Bild und Link einbauen

**Aufgabe:** Füge ein Bild ein und verlinke auf eine andere Webseite.

### 💡 Lösung:
```html
<img src="https://via.placeholder.com/150" alt="Platzhalter-Bild">
<p>Besuche <a href="https://www.google.com">Google</a>.</p>
```

🧠 **Erklärung:**
- `<img>` zeigt ein Bild an. `src` ist der Pfad, `alt` der Alternativtext.
- `<a>` ist ein Link. Das `href`-Attribut bestimmt das Ziel.

---

## ✅ Übung 3: Liste mit 3 Punkten

**Aufgabe:** Erstelle eine ungeordnete Liste mit drei Lieblingsessen.

### 💡 Lösung:
```html
<ul>
  <li>Pizza</li>
  <li>Sushi</li>
  <li>Pasta</li>
</ul>
```

🧠 **Erklärung:**
- `<ul>` ist eine ungeordnete Liste (Bullet Points).
- `<li>` sind die einzelnen Listenelemente.

---

## ✅ Übung 4: Eigene CSS-Datei erstellen

**Aufgabe:** Erstelle eine `style.css` und binde sie ein.

### 💡 HTML:
```html
<head>
  <link rel="stylesheet" href="style.css">
</head>
```

### 💡 style.css:
```css
body {
  font-family: Arial, sans-serif;
  background-color: #f0f0f0;
}
```

🧠 **Erklärung:**
- Mit `<link>` bindest du eine externe CSS-Datei ein.
- CSS regelt das Aussehen deiner Seite.

---

## ✅ Übung 5: Flexbox Layout mit 2 Spalten

**Aufgabe:** Baue ein Layout mit zwei nebeneinanderstehenden Boxen.

### 💡 HTML:
```html
<div class="container">
  <div class="box">Box 1</div>
  <div class="box">Box 2</div>
</div>
```

### 💡 CSS:
```css
.container {
  display: flex;
  gap: 20px;
}
.box {
  background-color: lightblue;
  padding: 20px;
  flex: 1;
}
```

🧠 **Erklärung:**
- `display: flex` macht ein flexibles Layout.
- `flex: 1` sorgt dafür, dass beide Boxen gleich breit sind.

---

## ✅ Übung 6: Navigation mit Hover-Effekt

**Aufgabe:** Baue eine horizontale Navigation mit Hover-Farbe.

### 💡 HTML:
```html
<nav>
  <ul class="nav">
    <li><a href="#">Home</a></li>
    <li><a href="#">Über uns</a></li>
    <li><a href="#">Kontakt</a></li>
  </ul>
</nav>
```

### 💡 CSS:
```css
.nav {
  list-style: none;
  display: flex;
  gap: 20px;
  padding: 0;
}
.nav li a {
  text-decoration: none;
  color: black;
}
.nav li a:hover {
  color: red;
}
```

🧠 **Erklärung:**
- `hover` bedeutet: Wenn man mit der Maus darüber fährt.
- `list-style: none` entfernt die Bullet Points.

---

## ✅ Übung 7: Formular mit Eingabefeldern

**Aufgabe:** Erstelle ein Formular mit Name, E-Mail und Nachricht.

### 💡 HTML:
```html
<form>
  <label for="name">Name:</label>
  <input type="text" id="name"><br>

  <label for="email">E-Mail:</label>
  <input type="email" id="email"><br>

  <label for="message">Nachricht:</label><br>
  <textarea id="message" rows="4" cols="30"></textarea><br>

  <button type="submit">Senden</button>
</form>
```

🧠 **Erklärung:**
- `<input>` für Texteingaben, `<textarea>` für mehrzeilige Texte.
- `label` ist beschriftend und erhöht die Benutzerfreundlichkeit.

---

## ✅ Übung 8: Grid-Galerie

**Aufgabe:** Erstelle eine Bildergalerie mit CSS Grid.

### 💡 HTML:
```html
<div class="gallery">
  <img src="https://via.placeholder.com/100">
  <img src="https://via.placeholder.com/100">
  <img src="https://via.placeholder.com/100">
</div>
```

### 💡 CSS:
```css
.gallery {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 10px;
}
.gallery img {
  width: 100%;
}
```

🧠 **Erklärung:**
- `grid-template-columns` bestimmt Spaltenanzahl.
- `1fr` bedeutet: gleiche Breite.

---

## ✅ Übung 9: Tabelle gestalten

**Aufgabe:** Erstelle und style eine einfache Tabelle.

### 💡 HTML:
```html
<table>
  <tr>
    <th>Name</th>
    <th>Alter</th>
  </tr>
  <tr>
    <td>Lena</td>
    <td>22</td>
  </tr>
  <tr>
    <td>Tom</td>
    <td>25</td>
  </tr>
</table>
```

### 💡 CSS:
```css
table {
  border-collapse: collapse;
  width: 100%;
}
th, td {
  border: 1px solid gray;
  padding: 8px;
  text-align: left;
}
```

🧠 **Erklärung:**
- `border-collapse` sorgt für ein einheitliches Tabellenlayout.
- Tabellen können Inhalte übersichtlich darstellen.

---

## ✅ Übung 10: Seite responsive machen

**Aufgabe:** Füge eine Media Query ein, um das Layout auf kleineren Geräten anzupassen.

### 💡 CSS:
```css
body {
  font-size: 16px;
}

@media (max-width: 600px) {
  body {
    font-size: 14px;
    background-color: lightgray;
  }
}
```

🧠 **Erklärung:**
- `@media` prüft die Bildschirmbreite.
- So kannst du Layout und Design an Smartphones anpassen.



