# Lighting
![Light Balancing](images/lightbalancing.png)

Um die gewünschte Lichtstimmung zu realisieren, werden mehrere kleinere Steh-Lampen eingesetzt. Dazu wird die Szene von vier kleinen Lichtquellen knapp unter der Decke erleuchtet, die eine Art Kronleuchter immitieren sollen. Durch mehrere Lichtquellen erscheinen die Schatten nicht zu kantig.

Zum besseren Anpassen der Lichtstärken der einzelnen Lampen aneinander kommt ein simpler Grau-Shader (Standard VrayMtl) zum Einsatz.

## Steh-Lampen
bestehend aus kleiner VrayLightSphere innen und einem VrayLightMesh für den Lampenschirm

![Screenshot Steh-Lampen](images/screenshot-leuchter.png)

**Anzahl:** 4

**VrayLightSpheres:**
1.0 Watt, 4000 K, Radius 1.0

**VrayLightMesh:**
0.1 Watt, 2700 K


## Deckenlampen
zwei unterschiedliche Leuchtstärken bei mehreren Positionen

![Screenshot Deckenlampen](images/screenshot-deckenlampen-markierungen.png)

### Kronleuchter-Immitat
(gelbe Markierung im Screenshot)
**Anzahl:** 3

**VrayLightSphere:**
2 Watt, 4000 K, Radius 2.0


### Zusätzliche Lampen als Aufhelllichter
**Anzahl:** 5 (grüne und rote Markierungen im Screenshot)

**VrayLightSphere:**
2 Watt, 4000 K, Radius 2.0

Zusätzlich 2 VrayLightRect Flächen (je 10x10 Groß, 1 Watt, 2132 K) zur Beleuchtung des Gangs hinter der Glasscheibe zum "Frühstücksraum" (linke Seite im Bild, siehe Rendering)
