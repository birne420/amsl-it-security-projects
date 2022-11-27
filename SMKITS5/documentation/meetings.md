# Meeting- und Fortschrittsprotokoll (SMK-Aspekt)
<table>
  <tbody>
    <tr>
      <th>Datum</th>
      <th>Meeting</th>
      <th>Anmerkungen/Inhalt</th>
      <th>Fragen</th>
    </tr>
    <tr>
      <td>KW 41<br />Mi, 12.10.2022</td>
      <td>Vorlesung: Themen</td>
      <td>
        <ul>
          <li>Themenvorstellung, Aufgabenverständnis, Einteilung</li>
        </ul>
      </td>
      <td>-</td>
    </tr>
    <tr>
      <td>KW 42<br />Mi, 19.10.2022</td>
      <td>Vorlesung: Grundlagen</td>
      <td>
        <ul>
          <li>Grundlagen-Vorlesung (<a href="https://elearning.ovgu.de/mod/resource/view.php?id=388327">Folien</a>), Tipps für späteren Bericht</li>
          <li>Folie 29: Attributierung relevant als Gegenmaßnahme? (Motivation/Stand der Technik)</li>
          <li>Folie 32: Wie kann Angreifer gegen Attributierung arbeiten, wenn er mehr Resourcen (Zeit, Geld, Rechenleistung) hat?</li>
          <li>Folie 33: Basisangriff einordnen</li>
          <li>Folie 56: Einordnen der These (Ausblick)</li>
          <li>Folie 59: zu untersuchenden Datenstrom einordnen (Konzept)</li>
        </ul>
      </td>
      <td>-</td>
    </tr>
    <tr>
      <td>KW 43<br />Mi, 26.10.2022</td>
      <td>Vorlesung: Einführung in Steganographie</td>
      <td>
        <ul>
          <li>TODO: Folie ausarbeiten</li>
        </ul>
      </td>
      <td>-</td>
    </tr>
    <tr>
      <td>KW 43<br />Sa, 29.10.2022</td>
      <td>Discord-Meeting (Bernhard, Ulrich)</td>
      <td>
        <ul>
          <li>Problem: Docker-Setup</li>
          <li>Script-Prototyp (Version 1)</li>
        </ul>
      </td>
      <td>-</td>
    </tr>
    <tr>
      <td>KW 43<br />Fortschritte</td>
      <td>Bernhard, Ulrich</td>
      <td>
        <ul>
          <li>Aufsetzen der Docker-Umgebung</li>
          <li><a href="www.citi.umich.edu/u/provos/papers/detecting.pdf">Referenz</a> gelesen: Attributierung</li>
          <li>alternative Bilddatenbank: <a href="https://www.kaggle.com/competitions/alaska2-image-steganalysis/data">Kaggle/Alaska2</a>, da BOWS nur pgm format</li>
        </ul>
      </td>
      <td>-</td>
    </tr>
    <tr>
      <td>KW 44<br />Di, 01.11.2022</td>
      <td>Task-Coach-Meeting (Bernhard, Christian)</td>
      <td>
        <ul>
          <li>Umwandeln von PGM-Bildern zu JPEG Bildern mit ImageMagick</li>
          <li>in Referenz-Paper sei genau eine Möglichkeit beschrieben, die wir untersuchen sollen</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>Probleme: Referenz-Links tot, Formate falsch</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>KW 44<br />Do, 03.11.2022</td>
      <td>Discord-Meeting (Bernhard, Ulrich)</td>
      <td>
        <ul>
          <li>Erarbeitung des <a href="./SMKITS-Presentation DR1.pdf">DR1-Foliensatzes</a></li>
          <li>Feedback von Christian angefordert</li>
        </ul>
      </td>
      <td>-</td>
    </tr>
    <tr>
      <td>KW 44<br />Fortschritte</td>
      <td>Bernhard, Ulrich</td>
      <td>
        <ul>
          <li>2 Shell-Scripte: Docker für Umgebung, Attributierungsscript für Stego-Untersuchung</li>
          <li>Bildtestset zusammenstellen begonnen &rarr; verschiedene Quellen werden benötigt</li>
          <li>Bildattributierungsmerkmale aus Referenz ausarbeiten: Erkennung von Manipulation in JPEG durch Betrachten der DCT-Koeffizienten
            <ul>
              <li>DCT: Discrete Cosine Transform</li>
              <li>Darstellung von 8x8 Pixel-Blöcken &rarr; Änderung der LSBs der Koeffizienten ist für Auge nicht erkennbar</li>
              <li>Einbettung sukzessive möglich, aber auch pseudo-zufällig &rarr; Unterschiede zwischen Tools</li>
            </ul>
          </li>
          <li>Überarbeitung des <a href="./SMKITS-Presentation DR1.pdf">DR1-Foliensatzes</a></li>
          <li>Einarbeitung in die zu verwendenden Tools</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>PGM-Bildformat in BOWS2-DB?</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>KW 45<br />Di, 08.11.2022</td>
      <td>Discord-Meeting (Bernhard, Ulrich)</td>
      <td>
        <ul>
          <li>Einteilung der Präsentation</li>
        </ul>
      </td>
      <td>-</td>
    </tr>
    <tr>
      <td>KW 45<br />Mi, 09.11.2022</td>
      <td>DR1-Präsentation</td>
      <td>
        <ul>
          <li>für stat. Signifikanz viele Bilder nötig &rarr; mindestens mehrere Hundert nötig</li>
          <li>Discord-Nachbesprechung: Einigung auf 1024 Bilder</li>
        </ul>
      </td>
      <td>-</td>
    </tr>
    <tr>
      <td>KW 45<br />Fr, 11.11.2022</td>
      <td>Discord-Meeting (Bernhard, Ulrich)</td>
      <td>
        <ul>
          <li>Aufgaben-Einteilung Bernhard: jphide-Fix (interaktive Eingabe automatisieren), Script</li>
          <li>Aufgaben-Einteilung Ulrich: Überlegungen zur Auswertung</li>
          <li>Erstellung GitHub-Repo</li>
        </ul>
      </td>
      <td>-</td>
    </tr>
    <tr>
      <td>KW 45<br />Fortschritte</td>
      <td>Bernhard</td>
      <td>
        <ul>
          <li>Ansatz: inhaltsunabhängig mit zufälligen Bildern, dabei Variationen nach Testprotokoll (Tools, Schlüssel, Inhalt)</li>
          <li>Einbettungen, dann Analyse, Ergebnisse mit Originalbild vergleichen, systematisches Vorgehen</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>Möglichkeit, wie man inhaltsbasierte Merkmale auslesen kann?</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>KW 46<br />Di, 15.11.2022</td>
      <td>Task-Coach-Meeting (Bernhard, Christian, Ulrich)</td>
      <td>
        <ul>
          <li>Script: Speicherplatzproblem, wenn erst alle Analysedaten erzeugt werden &rarr; Einbettungen erzeugen &rarr; analysieren &rarr; auswerten &rarr; löschen</li>
          <li>Problem mit Outguess-Binärdaten.. zu groß?</li>
          <li></li>
          <li>konzeptuelle Überlegungen sowie Vortests dokumentieren</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>Tool für Differenzbildberechnung? &rarr; ImageMagick/compare</li>
          <li>jphide-Problem: kein Passwort-Support</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>KW 46<br />Mi, 16.11.2022</td>
      <td>Vorlesung: Wissenschaftliches Schreiben</td>
      <td>
        <ul>
          <li>TODO: Folien durcharbeiten</li>
        </ul>
      </td>
      <td>-</td>
    </tr>
    <tr>
      <td>KW 46<br />Fortschritte</td>
      <td>Bernhard</td>
      <td>
        <ul>
          <li>Script umschreiben entsprechend Dienstags-Meeting (Version 2)</li>
          <li>Finalisieren des Bildtestsets (192+192+640=1024 Bilder)</li>
        </ul>
      </td>
      <td>-</td>
    </tr>
    <tr>
      <td>KW 47<br />Di, 22.11.2022</td>
      <td>Task-Coach-Meeting (Bernhard, Christian, Ulrich)</td>
      <td>
        <ul>
          <li>finalisiertes Bildtestset</li>
          <li>Werkzeugauswahl finalisiert</li>
          <li>Testziel-Tabelle</li>
          <li>Script-Fortschritt (Version 3): Auswertung der Daten direkt nach Einbettungserzeugung (gezielte Tool-Anwendung), alle Tools implementiert (jphide/stegbreak-Seg-Faults)</li>
          <li>Abschlussreport-Ausblick: Netze für höhere stat. Sign. und inhaltsbasierte Betrachtung, bessere Differenzbildanalyse &rarr; weiterführende Codeuntersuchungen (Contentanalyse)</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>jphide-Fix: Ausführung in Docker funktioniert nicht &rarr; statische Kompilierung</li>
          <li>StegBreak SegFault (immer, <a href="https://www.linux-community.de/ausgaben/linuxuser/2008/04/stegdetect-und-stegbreak/2/">Referenz</a>)</li>
          <li>strings-auswertung? &rarr; Fokus auf Unterschiede im Header</li>
          <li>Stegoveritas-Auswertung &rarr; Differenzbilder aller erzeugten Veritas-Bilder mit Original</li>
          <li>Schwarzes Differenzbild &rarr; Hervorgerufen von LSB-Frequenzraum-Pixel-Übersetzung</li>
          <li>Ablaufdiagramm klären &rarr; Ablauf der Analyse</li>
          <li>Dockerfile</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>KW 47<br />Fortschritte</td>
      <td>Bernhard, Christian, Ulrich</td>
      <td>
        <ul>
          <li>erneuter jphide-Fix-Versuch</li>
          <li>stegbreak-Fix-Versuch</li>
          <li>Attribute ausgearbeitet</li>
          <li>Evaluation angefangen</li>
        </ul>
      </td>
      <td>-</td>
    </tr>
    <tr>
      <td>KW 48<br />Di, 29.11.2022</td>
      <td>Task-Coach-Meeting (Bernhard, Christian, Ulrich)</td>
      <td>
        <ul>
          <li>jphide/jpseek SegFault-Problem, funktioniert nicht...</li>
          <li>stegbreak SegFault-Problem sehr häufig, einige wenige Analysen funktionieren aber...</li>
          <li>tabelle und diagramm präsentieren und feedback einholen</li>
          <li>Überspringen von f5 und stegoveritas-Analyse bei Bildern größer als 1024x1024: aktuell 5 min pro Bild &rarr; 12 bilder pro Stunde -> 288 Bilder pro Tag -> gut 3.5 Tage Analyse für alle 1024 Bilder</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>lange Einbettungslänge abhängig von Bildgröße? (8tel der Bilddateigröße)?</li>
          <li>Parallelisierung/Ausführung auf Cluster &rarr; Slurm-Script</li>
          <li>Attributietungsmerkmale auf "Vollständigkeit" überprüfen (stegoveritas gaussianblur? smooth? sharpened?)</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>