# UnitPulse

Free online conversion tools. Sister site of [NetPulse](https://janvanhal.github.io/netpulse/).

Vanilla HTML, CSS and JavaScript. No build step and no account. Each tool is one page, and the script for that tool is in the page.

## Run locally

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8080
```

Then open http://localhost:8080/

The currency converter asks [Frankfurter](https://www.frankfurter.app/) for European Central Bank reference rates. Browsers cannot follow the redirect from `api.frankfurter.app` to `api.frankfurter.dev`, so the page tries the first address and then the second. That works from a local server or from GitHub Pages. If both fail, the page uses rates saved in the browser, or a built-in table from 9 October 2026 labelled approximate, offline. The other tools work with no network.

Published site: https://janvanhal.github.io/unitpulse/

## Pages

| File | Page |
|------|------|
| `index.html` | Home: eight tools, then the introduction, then the blog |
| `currency.html` | Currency, live ECB rates via Frankfurter, default THB and EUR |
| `length.html` | Length, including feet and inches |
| `weight.html` | Weight, including pounds and ounces |
| `temperature.html` | Celsius, Fahrenheit, kelvin |
| `volume.html` | Cooking volume and ingredient grams |
| `area.html` | Area, including rai, ngan and square wa |
| `speed-fuel.html` | Speed and fuel economy |
| `timezone.html` | Time zones, with daylight saving via the browser |
| `blog.html` | Blog index |
| `blog/*.html` | Articles. They link `../styles.css` |
| `about.html` | About |
| `contact.html` | Contact. Opens your email app |
| `privacy.html` | Privacy |
| `terms.html` | Terms |
| `dmca.html` | Copyright notices |
| `styles.css` | Notion warm-paper styles shared with NetPulse, plus converter components at the end |
| `img/unitpulse-icon.svg` | Icon and favicon |
| `img/unitpulse-logo.svg` | Homepage logo |

Ad slots use the placeholder publisher ID `ca-pub-1234567890`. The AdSense script is not loaded, so the placeholder does not throw in the console.

The contact address `contact@unitpulse.example` is a placeholder.
