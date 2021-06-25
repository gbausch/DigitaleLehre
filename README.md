# Digitale Lehre

Diese Seite dokumentiert meine Erfahrungen sowie Werkzeuge und Workflows zur Erstellung digitaler Lehrinhalte, die ich im Sommersemester 2020 zusammengetragen habe.

## Ausrüstung
- MacBookPro 13 Zoll (2019)
- iPad Air (4. Generation) inkl. Apple Pencil
- ~Microsoft Surface inkl. Stift~
- Headset: [Sennheiser PC 360](https://amzn.to/2TdXJ6f)
- Dokumentenkamera: [IPEVO VZ-X8M](https://www.ipevo.com/products/vz-x)

## Software
### Präsentation
- [Apple Keynote](https://www.apple.com/de/keynote/) zur Erstellung von Präsentationen (Export als PDF)
- [GoodNotes](https://www.goodnotes.com) für Präsentation und Notizen
- [AirServer](https://www.airserver.com) iPad -> MacOS -> Freigabe in [Zoom](https://zoom.us)

### Aufzeichnung von Videos
- [OBS Studio](https://obsproject.com/de/)
- [Apple iMovie](https://www.apple.com/de/imovie/)
- [Youtube](https://youtube.com)

## Workflow für Videos
1. Erstellung von Präsentationsfolien mit Keynote
2. Export der Keynote-Präsentationen als PDF (jede Animationsstufe einzeln)
3. Aufnahme mit OBS auf Surface (wenn Stiftunterstützung notwendig ist)
4. Videoschnitt auf Mac (iMovie)
5. Kompression mit `ffmpeg` auf Mac: `ffmpeg -i <INPUT.mp4> -c:a copy -c:v libx264 <OUTPUT.mp4>`
6. Thumbnail für Youtube extrahieren: `ffmpeg -i <INPUT.mp4> -vframes 1 thumbnail.jpg`
7. Upload auf Youtube mit nicht-öffentlichem Link

## Gedanken
- ~Das Microsoft Surface inkl. Stift nutze ich zur Aufnahme von Video, Audio und handschriftlichen Notizen, die ich in die Präsentationen mache. Wenn ich diese Aufgaben mit einem iPad erledigen kann, ist das Surface obsolet.~

## Weitere nützliche Werkzeuge
- [JupyterLab](https://jupyter.org)
- ~[Whiteboard.com](https://witeboard.com/)~
- [Slido](https://www.sli.do/de)
- [Mentimeter.com](https://www.mentimeter.com)
