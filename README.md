# Digitale Lehre

Diese Seite dokumentiert meine Erfahrungen sowie Werkzeuge und Workflows zur Erstellung digitaler Lehrinhalte, die ich im Sommersemester 2020 zusammengetragen habe.

## Ausrüstung
- MacBookPro 13 Zoll (2019)
- Microsoft Surface inkl. Stift
- Headset: [Sennheiser PC 360](https://amzn.to/2TdXJ6f)
- Dokumentenkamera: [IPEVO VZ-X8M](https://www.ipevo.com/products/vz-x)

## Software
- [OBS Studio](https://obsproject.com/de/)
- [Apple iMovie](https://www.apple.com/de/imovie/)
- [Youtube](https://youtube.com)

## Workflow
1. Erstellung von Präsentationsfolien mit Keynote
2. Export der Keynote-Präsentationen als PDF (jede Animationsstufe einzeln)
3. Aufnahme mit OBS auf Surface (wenn Stiftunterstützung notwendig ist)
4. Videoschnitt auf Mac (iMovie)
5. Kompression mit `ffmpeg` auf Mac: `ffmpeg -i <INPUT.mp4> -c:a copy -c:v libx264 <OUTPUT.mp4>`
6. Thumbnail für Youtube extrahieren: `ffmpeg -i <INPUT.mp4> -vframes 1 thumbnail.jpg`
7. Upload auf Youtube mit nicht-öffentlichem Link

## Gedanken
- Das Microsoft Surface inkl. Stift nutze ich zur Aufnahme von Video, Audio und handschriftlichen Notizen, die ich in die Präsentationen mache. Wenn ich diese Aufgaben mit einem iPad erledigen kann, ist das Surface obsolet.
