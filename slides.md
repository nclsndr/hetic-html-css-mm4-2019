---
title: HTML / CSS - MM4
verticalSeparator: <!--v-->
theme: solarized
revealOptions:
    transition: 'slide'
    transitionSpeed: 'fast'
---

## MM4

# HTML / CSS

Note:
https://nclsndr.github.io/hetic-html-css-mm4-2019
---

## Who am I?

- [Nicolas André](https://twitter.com/nclsndr) — UX Engineer at <a target="_blank" href="https://www.chance.co">Chance</a>

---

# And you?

---

## About this cycle

26 nov. <br>
[Internet](#/8) - [The Web](#/25) - [HTML](#/35) - [CSS](#/47) - [Dev tools](#/57) <br>
03 dec. <br>
10 dec. <br>
Sandboxes: [Basis](#/43) - [HTML/CSS](#/52)
---

<h1 style="color: #FFF;">Ready?</h1>

<!-- .slide: data-background="assets/ready.gif" -->

---

# 🧐

### Who is HTML?

---

### Some valid definition 

by [Mozilla docs](https://developer.mozilla.org/en-US/docs/Web/HTML)

__HTML__ (HyperText Markup Language) is the most basic building block of the Web. It defines the meaning and structure of web content. [...]

---

# 🤷‍♀️
### Ok, but why?

---

<h2 style="color: #FFF;">Back in 1969</h2>

<!-- .slide: data-background="https://media.giphy.com/media/3o7aD46cTjbkp0gT5e/giphy.gif" -->
---

<div>
  <img src="assets/cold_war_1970.png">
</div>

### 🇺🇸 👮‍♀️ 💬 ☢️ 💬 👨‍💼
---

<img style="height: 300px" src="assets/darpa_logo.jpg">

[Defense Advanced Research Projects Agency](https://www.darpa.mil/about-us/about-darpa) — since 1958
---
<div>
  <img style="width: 20%; margin: 3%;" src="assets/standford_logo.png">
</div>

## SRI
[Stanford Research Institute](https://en.wikipedia.org/wiki/SRI_International) — since 1946

---
<div>
  <img style="width: 20%; margin: 3%;" src="assets/engelbart.webp">
</div>

### [Douglas Engelbart](https://en.wikipedia.org/wiki/Douglas_Engelbart)

American engineer and inventor, and early computer and Internet pioneer

Founder of Augmentation Research Center (ARC) at SRI

---
<div>
  <img style="width: 16%; margin: 3%;" src="assets/standford_logo.png">
  <img style="width: 16%; margin: 3%;" src="assets/ucla_logo.png">
</div>
<div>
  <img style="width: 16%; margin: 3%;" src="assets/utah_logo.png">
  <img style="width: 16%; margin: 3%;" src="assets/ucsb_logo.jpg">
</div>

### 🧑‍🏫 📺 💬 📺 🧑‍🏫

Note:
https://www.lib.utah.edu/digital-scholarship/arpanet/
https://en.wikibooks.org/wiki/The_Computer_Revolution/Networks/Internet

---
> The goal was to exploit new computer technologies to meet the needs of military command and control against nuclear threats, achieve survivable control of US nuclear forces, and improve military tactical and management decision making.

*— [Stephen J. Lukasik](https://en.wikipedia.org/wiki/ARPANET#Debate_on_design_goals), Director of DARPA (1967–1974)*

---
> The ARPANET was not started to create a Command and Control System that would survive a nuclear attack, as many now claim. [...]. Rather, the ARPANET came out of our frustration that there were only a limited number of large, powerful research computers in the country, and that many research investigators, who should have access to them, were geographically separated from them.

*— [Charles Herzfeld](https://en.wikipedia.org/wiki/ARPANET#Debate_on_design_goals), ARPA Director (1965–1967)*

---
### [Request For Comments](https://tools.ietf.org/html/rfc1)

<div>
  <img src="assets/rfc1.png">
</div>

Applying scientific method for a collaborative definition of protocols

---
<div>
  <img src="assets/arpanet69.jpg">
</div>

1969
---
<div>
  <img src="assets/arpanet70.jpg">
</div>

1970
---
<div>
  <img src="assets/arpanet73.jpg">
</div>

1973 - [source: vox.com](https://www.vox.com/a/internet-maps)
---
<!-- .slide: data-background="assets/twitter_wake_up.gif" -->
---

## Internet VS Web?

---

### RFC1122 - Internet Protocol Suite

<div>
  <img src="assets/tcp_ip_stack.png">
</div>

---
### Internet is a set of network protocols

### The Web is an abstract application on top of it
---
<!-- .slide: data-background="assets/the-web.jpg" -->
---
# The web
---
### Who's that guy?

<div>
  <img src="assets/Tim.png">
</div>
---

<div>
  <img style="width: 200px;" src="assets/Tim.png">
</div>

### [Tim Berners-Lee](https://en.wikipedia.org/wiki/Tim_Berners-Lee)

English engineer and computer scientist — CERN researcher
---

## 🧑‍🔬 ✉️ 📡 📞 📬 🧑‍🔬 🤯

Berners-Lee observed how hard it was to share information amoung researches — Especially linking articles

---
## His solution?
---
<code class="large">
  HyperText Markup Language
</code>

<div>
  <img src="assets/HyperText.png">
</div>
---
### Ok, but IRL it looks more like 👉
---
<div>
  <img src="assets/web_flow.png">
</div>
---
### ...with HTTP and so on!?
---
<h2 style="color: #FFF;">Yes, but that's another story...</h2>
<!-- .slide: data-background="assets/close_curtain.gif" -->
---

# HTML

## The web building block
---
<div>
  <img src="assets/simple_html_page.png">
</div>
---
<!-- .slide: data-background="assets/matrix_code.gif" -->

# 👇

<h2 style="color: #FFF;">cmd + alt + I</h2>
---

### HTML is a markup language based on XML

[Extensible Markup Language (XML)](https://en.wikipedia.org/wiki/XML)

---
### It's all about boxes containing boxes

<div>
  <img src="assets/xml_example.png">
</div>
---

### HTML Element

<div class="markup">
  <pre>&lt;</pre><span class="markup__tagname">tag</span> <br>
  &nbsp;&nbsp;<span class="markup__attribute">attribute</span><span>="value"</span><br>
  <pre>&gt;</pre><br>
  &nbsp;&nbsp;<span class="markup__content">Content?</span><br>
  <pre>&lt;/</pre><span class="markup__tagname">tag</span><pre>&gt;</pre><br>
</div>

---

### Common HTML tags

```html
<html>Document root</html>
<head>Document meta header</head>
<body>Page content</body>
<div>Default container</div>
<h1>Heading 1</h1>...<h6>Heading 6</h6>
<p>Paragraph</p>
<a>HyperText link</a>
<form>Form of user inputs</form>
<header>Header component</header>
<footer>Footer component</footer>
<nav>Containing navigation items</nav>
...
```
---
### HTML5 minimal page

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8" />
        <title>Titre</title>
    </head>

    <body>
    
    </body>
</html>
```
---
<iframe
  class="codesandbox"
  src="https://codesandbox.io/embed/sleepy-edison-jeq14?autoresize=1&fontsize=14&hidenavigation=1&theme=dark"
  title="html-basis"
  allow="geolocation; microphone; camera; midi; vr; accelerometer; gyroscope; payment; ambient-light-sensor; encrypted-media; usb"
  sandbox="allow-modals allow-forms allow-popups allow-scripts allow-same-origin"
></iframe>

Note:
Build basic information display of article (Title, p, image)
---
# ✋
### Ok, but all this looks pretty ugly right?
---
How to get from
<div>
  <img src="assets/hetic_no_css.png">
</div>
---
To
<div>
  <img src="assets/hetic_css.png">
</div>
---

# HTML ❤️ CSS

```html
<link href="styles/style.css" rel="stylesheet">
```
---

## CSS

[Cascading Style Sheet](https://developer.mozilla.org/en-US/docs/Web/CSS)

```css
p {
  color: red;
}
.title {
  font-style: 2rem;
}
```
---

### Selectors

```html
<body>
    <p class="someClass">
        <span id="someIdentifier">Foo</span>
    </p>
    <p class="someClass">Bar</p>
</body>
```

```css
/* HTML tags: tag selector */
body { margin: 0 }

/* HTML class attribute: class selector */
.someClass { color: blue; }

/* HTML id attribute: id selector */
#someIdentifier { font-size: 8rem; }
```
---

### Properties

```css
p {
  display: block;
  color: #000;
  font-family: "Helvetica", "Arial", sans-serif;
  border: none;
  font-style: normal;
  font-size: 1rem;
  font-weight: bold;
  line-height: 1.3em;
  /* ... */
}
```

[CSS Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference)
---
### Pseudo-selectors

```html
<a class="someLink" href="/any">Some link</a>
```

```css
.someLink { color: white; }
.someLink:hover { color: black; }
.someLink:active { color: blue; }
.someLink:visited { color: blue; }
```

[Pseudo-class docs](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes)
---

<iframe
  class="codesandbox"
  src="https://codesandbox.io/embed/html-css-basis-ee5d0?fontsize=14&hidenavigation=1&theme=dark"
  style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;"
  title="html-css-basis"
  allow="geolocation; microphone; camera; midi; vr; accelerometer; gyroscope; payment; ambient-light-sensor; encrypted-media; usb"
  sandbox="allow-modals allow-forms allow-popups allow-scripts allow-same-origin"
></iframe>

Note:
Flux Display /Inheritance / selector depth
---
## Think in boxes 👉
---
<div>
  <img src="assets/fb5.jpg">
</div>
---
<div>
  <img src="assets/fb5_1.jpg">
</div>
---
<div>
  <img src="assets/fb5_2.jpg">
</div>
---

# 🛠
## Some dev tools to continue

---
<div>
  <img style="width: 150px;" src="assets/vscode_logo.png">
</div>

## VS Code

Simple code editor

[https://code.visualstudio.com/download](https://code.visualstudio.com/download)

---
<div>
  <img style="width: 250px;" src="assets/nodejs_logo.png">
</div>

## NodeJS

Javascript runner

[https://nodejs.org/en/download/](https://nodejs.org/en/download/)

---
<div>
  <img style="width: 260px;" src="https://www.macworld.co.uk/cmsdata/features/3608274/Terminalicon2_thumb800.png">
</div>

## Terminal

```bash
$ node -v
$ npm -v
```
---
<div>
  <img style="width: 150px;" src="assets/code_sandbox_logo.png">
</div>

## Code Sandbox

Collaborative online editor

[https://codesandbox.io/](https://codesandbox.io/)

---

# ⚠️
## TODO: Missing repo to clone

---

# 👷
## Let's code

---
<div>
  <img src="assets/basic_profile.png">
</div>
---

# Resources

---

### Dev tools

[caniuse.com](https://caniuse.com)

---

## That's all folks

Thank you
